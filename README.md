<!--
SPDX-FileCopyrightText: 2022 Julia Rohrer, Karsten Lübke
SPDX-FileContributor: 2024-2025 Johannes Keyser

SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Einführungskurs Kausale Inferenz

## Beschreibung

Dieses Projekt enthält Materialien des Kurses _Was, wie, warum? - Einführungskurs Kausale Inferenz_ von [Dr. Julia Rohrer](https://juliarohrer.com/) (Universität Leipzig) und [Prof. Dr. Karsten Lübke](https://ki-campus.org/node/793) (FOM Hochschule).

### Hintergrund

Zum Studieren des Materials besuchen Sie am besten die ShinyApps der ursprünglichen Kursmaterialen, mit Einstieg unter <https://fomshinyapps.shinyapps.io/WWWEKI_Modul_01/>.
Die zugehörigen Interview-Videos finden Sie unter <https://wwweki.gitlab.io/interviews/>.

Der Kurs war bis Ende 2024 auf <https://ki-campus.org/> verfügbar, inklusive Prüfungsfragen; dieses Angebot wurde seitens KI-Campus gestoppt.

### Änderungen

Die hier enthaltenen, teilweise modifizierten Materialien sollen es Lehrkräften erleichtern, das Kursmaterial für den eigenen Unterricht anzupassen.

Dieses Projekt ist eine Kopie (ein _Fork_) von <https://github.com/luebby/WWWEKI>, mit folgenden (geplanten) Modifikationen:

- (Einige) HTML-Texte werden in Markdown umgewandelt.
- (Einige) Diagramme werden in SVG umgewandelt.
- Die ursprünglichen R-Markdown-Dateien (die Grundlage der ShinyApps) werden zusätzlich als IPython-Notebooks konvertiert.
    - Die Notebooks (mit Dateiendung `.ipynb`) erlauben, die Ergebnisse des Codes in derselben Datei im Webbrowser darzustellen, und erleichtern ggf. die Verwendung einer anderen Programmiersprache als R.
    - Die R-Markdown-Dateien (mit Endung `.Rmd`) sollen möglichst unverändert bleiben, für einfache Vergleichbarkeit mit dem ursprünglichen Projekt.
    - Zwischen den Dateiformaten und  kann dank [Jupytext](https://jupytext.readthedocs.io/) automatisch synchronisiert werden.  
- Beispieldatensätze werden als lokale CSV-Dateien bereitgestellt.

Eine genauere Aufschlüsselung der Änderungen finden Sie in Datei [CHANGELOG.md](CHANGELOG.md).

## Installation

Mit [Anaconda](https://anaconda.org/) können Sie mit einem Befehl alle benötigten und optionalen Pakete in einer neuen virtuellen Umgebung installieren:

```shell
conda create --name meinKI -c conda-forge jupyter jupytext r-irkernel r-tidyverse r-mosaic r-learnr r-ggthemes
```

Um das Material auf GitHub oder GitLab usw. zu betrachten wird nur ein Webbrowser benötigt.

Um die IPython-Notebooks (Dateien `*.ipynb`) auszuführen oder zu ändern, müssen Sie Jupyter (oder einen geeigneten Editor) installieren.

Sie müssen den `R`-Kernel für Jupyter installieren, um die R-Codezellen ausführen zu können.
Der Kurs stützt sich auf die R-Pakete `tidyverse` und `mosaic`, `learnr`, `ggthemes`, die ihrerseits zusätzliche Abhängigkeiten mit sich bringen.

Optional: Um das Material zwischen den Formaten R-Markdown und Jupyter-Notebook zu synchronisieren, wird [Jupytext](https://jupytext.readthedocs.io/) verwendet.

Optional: Um die Materialien in PDF-Handouts, Folien oder ein anderes Format zu konvertieren, können Sie [Quarto](https://quarto.org/) installieren (das [Pandoc](https://pandoc.org/) enthält, einen leistungsstarken Konverter, den Sie auch ohne Quarto verwenden können).

Optional: Um Ihre Änderungen zu verfolgen und zu diesem Projekt beizutragen, benötigen Sie Git.


## Modulübersicht

1. An der Weggabelung: Einen Weg gehen - und einen nicht (Potential Outcome und Counterfactual)
    - Interner Link auf Variante als [R-Markdown](Module/Modul_01.Rmd) und als [IPython Notebook](Module/Modul_01.ipynb)
    - Externer Link auf [ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_01/)

2. Ein Pfeil zeigt die Richtung (Strukturelle kausale Modelle und Kausale Diagramme)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_02/)

3. Daten analysieren – mit welchem Ziel? (Datenanwendungen (Beschreibung, Vorhersage, Kausale Inferenz), Kausale Leiter (Assoziation, Intervention, Counterfactual))
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_03/)

4. Es steht was zwischen uns (Kette)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_04/)

5. Von Störchen und Geburten (Gabel)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_05/)

6. Nett oder schön? – Warum nicht beides? (Umgedrehte Gabel)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_06/)

7. Warum Raumteilung keine gute Investition ist (Wiederholung Grundelemente Kausaler Diagramme, Unterschied (do(x) vs. X=x am Beispiel)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_07/)

8. Magie durch Zufall (Zufällige Stichprobe und zufällige Zuordnung im Rahmen eines Experiments und die Auswirkungen auf die Datenanwendungen (Beschreibung, Vorhersage, Kausale Inferenz) )
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_08/)

9. Was wäre gewesen, wenn? (Counterfactual)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_09/)

10. Graphen zeichnen und lesen (Beispiel Gender-Pay-Gap)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_10/)

11. Schadet Rauchen bei Heranwachsenden? (Anwendungsbeispiel Kausale Inferenz in der Medizin.)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_11/)

12. Praktisches Daten hinterfragen (DAGs in der Anwendung, Ausblick)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_12/)


## Weiterführende Links

- Eine englische Kursvariante ist verfügbar unter <https://github.com/luebby/WWWEKI-EN>.
- Details siehe z.B. [FOM forscht Wissenschaftsblog](https://www.fom-blog.de/2021/07/einstiegskurs-kausale-inferenz-wird-gemeinsam-von-der-universitaet-leipzig-und-der-fom-hochschule-mit-einer-foerderung-durch-das-bmbf-entwickelt/).
 
**Videos**:

- Die begleitenden Interviews mit angesehenen Expert:innen aus unterschiedlichen Fachgebieten, die ihre kausalen Fragestellungen und Lösungsansätze vorstellen, finden Sie unter <https://wwweki.gitlab.io/interviews/>.

**Literatur**:

- Rohrer, J. M. (2018). Thinking clearly about correlations and causation: Graphical causal models for observational data. *Advances in Methods and Practices in Psychological Science*, 1(1), 27-42. [https://doi.org/10.1177%2F2515245917745629](https://doi.org/10.1177%2F2515245917745629)
- Lübke, K., Gehrke, M., Horst, J., & Szepannek, G. (2020). Why we should teach causal inference: Examples in linear regression with simulated data. *Journal of Statistics Education*, 28(2), 133-139. [https://doi.org/10.1080/10691898.2020.1752859](https://doi.org/10.1080/10691898.2020.1752859)


## FIXME: Beitragen

Bitte melden Sie Fehler, Unklarheiten und Verbesserungsvorschläge beim originalen Projekt unter <https://github.com/luebby/WWWEKI/issues>.


## Lizenz

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Namensnennung - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz</a>.

## Förderung

Das Vorhaben *Was, wie, warum? Einstiegskurs Kausale Inferenz (WWWEKI)* wurde mit Mitteln des Bundesministeriums für Bildung und Forschung unter dem Förderkennzeichen `16DHBQP040` gefördert.

### Hintergrund

Im Rahmen der Kausalen Inferenz sind in den letzten Jahren sowohl in Wissenschaft als auch in der Praxis beachtliche Fortschritte erzielt worden.

Gleichzeitig wird das Thema Kausalität in vielen Forschungsfeldern entweder explizit ausgeklammert oder ignoriert.
Dies führt zu vielfältigen Problemen in der Datenanalyse (z. B. werden Quellen von Bias oft ignoriert) und es kommt zu einem Mismatch zwischen der gewählten Methode und der Frage, die eigentlich beantwortet werden soll (z. B. werden rein prädiktive Methoden verwendet, um letztlich kausale Fragen zu beantworten).
Das gilt auch für den Bereich der Künstlichen Intelligenz der von einem stärkeren Fokus auf Kausale Inferenz profitieren würde.

### Zielsetzung

Schon länger wird gefordert, dass das Thema Kausale Inferenz eine zentrale Rolle in den Lehrplänen spielen sollte.

Englischsprachig gibt es diverse (erfolgreiche) MOOCs zum Thema Kausale Inferenz, z. B. von edX, Udemy oder coursera.
Auch stehen diverse Bücher zu unterschiedlichen Anwendungsfeldern zum Einstieg zur Verfügung, so z. B. von Neal (2020): “Introduction to Causal Inference from a Machine Learning Perspective”, oder Peters, Janzing & Schölkopf (2017): “Elements of Causal Inference”.
Nicht zuletzt aufgrund der Aktualität des Themas gibt es nach bestem Wissen der Antragsteller:innen jedoch kein vergleichbares deutschsprachiges Angebot.
Diese Lücke soll der Kurs schließen.

### Methodik

Die ausgewählten Inhalte orientieren sich an Cummiskey & Lübke (2022):

- Elementare Grundlagen von Wahrscheinlichkeit und Statistik, insbesondere bedingte Wahrscheinlichkeiten und Unabhängigkeit
- Potential Outcome und Counterfactual
- Kausale Effekte und Verzerrungen (letztere auch bei rein deskriptiven Beschreibungen, z. B. Selection/Survivor Bias)
- Directed Acyclic Graphs als Mittel zur Beschreibung des datengenerierenden Prozesses
- Unterschiedliche Ebenen der Datenanwendung und ihre Voraussetzungen

Um den Kurs allgemein interessant zu gestalten, werden die Inhalte entlang von alltäglichen Beispielen motiviert und erklärt werden.
Themenbezogene kurze Videos, aber auch Animationen, sollen den Lernprozess unterstützen.
Im Rahmen des MOOCs werden dabei verschiedene offene und geschlossene Fragen inklusive Rückmeldung integriert.

### Publikationen

- Lübke, K., Gehrke, M., Horst, J., & Szepannek, G. (2020).
  Why we should teach causal inference: Examples in linear regression with simulated data.
  Journal of Statistics Education, 28(2), 133-139.
- Rohrer, J. M. (2018).
  Thinking Clearly About Correlations and Causation: Graphical Causal Models for Observational Data.
  Advances in Methods and Practices in Psychological Science, 1(1), 27–42.
- Cummiskey, K., & Lübke, K. (2022).
  Causality in Data Science Education.
  Submitted.

![Logo BMBF](/images/csm_Logo-BMBF.jpg)
