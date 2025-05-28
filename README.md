<!--
SPDX-FileCopyrightText: 2022 Julia Rohrer, Karsten Lübke
SPDX-FileContributor: 2024-2025 Johannes Keyser

SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Einführungskurs Kausale Inferenz

## Beschreibung

Dieses Projekt enthält Materialien des Kurses _Was, wie, warum? - Einführungskurs Kausale Inferenz_ von [Dr. Julia Rohrer](https://juliarohrer.com/) (Universität Leipzig) und [Prof. Dr. Karsten Lübke](https://ki-campus.org/node/793) (FOM Hochschule).

Zum Studieren des Materials besuchen Sie am besten die ShinyApps der ursprünglichen Kursmaterialen, siehe unter [Modulübersicht](#modulübersicht).

Der Kurs setzt sich zusammen aus Interviews mit Expert:innen aus unterschiedlichen Fachgebieten sowie interaktiven Tutorials.
Alle Interviews auf einen Blick finden Sie unter [https://wwweki.gitlab.io/interviews/](https://wwweki.gitlab.io/interviews/).
Die Interviews und Tutorials sind teilweise inhaltlich aufeinander abgestimmt, können aber auch problemlos in Isolation verwendet werden.

### Hintergrund

Der Kurs war bis Ende 2024 auf <https://ki-campus.org/> verfügbar, inklusive Prüfungsfragen; dieses Angebot wurde seitens KI-Campus beendet.

Dieser Kurs zum Einstieg in die Kausalinferenz wurde ursprünglich entwickelt als MOOC für den [KI-Campus](https://ki-campus.org/) in Kooperation zwischen Karsten Lübke (FOM Hochschule) und Julia Rohrer (Projektleitung, Universität Leipzig).

### Änderungen

Die hier enthaltenen Materialien sollen es Lehrkräften erleichtern, das Kursmaterial für den eigenen Unterricht anzupassen.
Dabei werden zunächst keine inhaltlichen Änderungen angestrebt.

Dieses Projekt ist eine Kopie (ein _Fork_) von <https://github.com/luebby/WWWEKI>, mit folgenden (geplanten) Änderungen:

- (Einige) HTML-Texte werden in Markdown umgewandelt.
- (Einige) Diagramme werden in SVG umgewandelt.
- Die ursprünglichen R-Markdown-Dateien (die Grundlage der ShinyApps) werden zusätzlich als IPython-Notebooks konvertiert.
  - Die Notebooks (mit Dateiendung `.ipynb`) erlauben, die Ergebnisse des Codes in derselben Datei im Webbrowser darzustellen, und erleichtern ggf. die Verwendung einer anderen Programmiersprache als R.
  - Die R-Markdown-Dateien (mit Endung `.Rmd`) sollen möglichst unverändert bleiben, für einfache Vergleichbarkeit der ursprünglichen Materialien.
  - Zwischen den Dateiformaten und kann dank [Jupytext](https://jupytext.readthedocs.io/) automatisch synchronisiert werden.
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
    - [Kurzes Video: Willkommen im Kurs](https://youtu.be/AthXheSZhXE)
2. Ein Pfeil zeigt die Richtung (Strukturelle kausale Modelle und Kausale Diagramme)
    - [Interview mit David Lagnado: Wie wir kausal danken](https://www.youtube.com/watch?v=Um0lkCA6Evk)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_02/)
3. Daten analysieren – mit welchem Ziel? (Datenanwendungen (Beschreibung, Vorhersage, Kausale Inferenz), Kausale Leiter (Assoziation, Intervention, Counterfactual))
    - [Interview mit Stephan Poppe: Die kausale Leiter](https://www.youtube.com/watch?v=2uHLEgdvZt4)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_03/)
4. Es steht was zwischen uns (Kette)
    - [Kurzes Video: Gabel, Kette, umgedrehte Gabel -- fundamentale kausale Strukturen](https://www.youtube.com/watch?v=A8kMmDd_qR8)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_04/)
5. Von Störchen und Geburten (Gabel)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_05/)
    - [Interview mit Anne: Wie beeinflusst das Stillen die kindliche Entwicklung?](https://www.youtube.com/watch?v=x7o4pjpcuxo)
6. Nett oder schön? – Warum nicht beides? (Umgedrehte Gabel)
    - [Interview mit Carla Schmitt: Kausalinferenz im Unternehmenskontext](https://www.youtube.com/watch?v=VZcwxd9fG10)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_06/)
7. Warum Raumteilung keine gute Investition ist (Wiederholung Grundelemente Kausaler Diagramme, Unterschied (do(x) vs. X=x am Beispiel)
    - [Interview mit Dean Eckles: Soziale Ansteckung](https://www.youtube.com/watch?v=Tr9TfyR19h8)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_07/)
8. Magie durch Zufall (Zufällige Stichprobe und zufällige Zuordnung im Rahmen eines Experiments und die Auswirkungen auf die Datenanwendungen (Beschreibung, Vorhersage, Kausale Inferenz) )
    - [Interview mit Richard McElreath: Kausales Denken für alle Datenanwendungen](https://www.youtube.com/watch?v=YvhuYONl1o0)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_08/)
9. Was wäre gewesen, wenn? (Counterfactual)
    - [Interview mit Sebastian Weichwald: Pragmatische Kausalinferenz](https://www.youtube.com/watch?v=0hDrxbpJsvY)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_09/)
10. Graphen zeichnen und lesen (Beispiel Gender-Pay-Gap)
    - [Interview mit Jakob Runge: Kausalinferenz in komplexen Klimasystemen](https://www.youtube.com/watch?v=HFoDVJOqFZw)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_10/)
11. Schadet Rauchen bei Heranwachsenden? (Anwendungsbeispiel Kausale Inferenz in der Medizin.)
    - [Interview mit Jonas Peters: Causal Discovery](https://www.youtube.com/watch?v=Dy6CutsvMbY)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_11/)
12. Praktisches Daten hinterfragen (DAGs in der Anwendung, Ausblick)
    - [Kurzes Video zum Abschied](https://youtu.be/UZwlsbEf2P0)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_12/)

## Weiterführende Links

- Eine englische Kursvariante ist verfügbar unter <https://github.com/luebby/WWWEKI-EN>.
- Für weitere Hintergründe zum Kurs siehe [FOM forscht Wissenschaftsblog](https://www.fom-blog.de/2021/07/einstiegskurs-kausale-inferenz-wird-gemeinsam-von-der-universitaet-leipzig-und-der-fom-hochschule-mit-einer-foerderung-durch-das-bmbf-entwickelt/).

### Video-Interviews

- Die begleitenden Interviews mit angesehenen Expert:innen aus unterschiedlichen Fachgebieten, die ihre kausalen Fragestellungen und Lösungsansätze vorstellen, finden Sie unter <https://wwweki.gitlab.io/interviews/>.

### Literatur

- Rohrer, J. M. (2018).
  Thinking clearly about correlations and causation: Graphical causal models for observational data.
  _Advances in Methods and Practices in Psychological Science_, 1(1), 27-42.
  <https://doi.org/10.1177%2F2515245917745629>
- Lübke, K., Gehrke, M., Horst, J., & Szepannek, G. (2020).
  Why we should teach causal inference: Examples in linear regression with simulated data.
  _Journal of Statistics Education_, 28(2), 133-139.
  <https://doi.org/10.1080/10691898.2020.1752859>

## Beitragen

Bitte melden Sie inhaltliche Fehler, Unklarheiten und Verbesserungsvorschläge beim ursprünglichen Projekt, unter <https://github.com/luebby/WWWEKI/issues>.

Weitere Vereinfachungen der Materialien zwecks Wiederverwendung in eigenen Kursen können Sie gerne auch hier vorschlagen.

## Lizenz

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Namensnennung - Weitergabe unter gleichen Bedingungen 4.0 International Lizenz</a>.

## Förderung

Das Vorhaben _Was, wie, warum? Einstiegskurs Kausale Inferenz (WWWEKI)_ wurde mit Mitteln des Bundesministeriums für Bildung und Forschung unter dem Förderkennzeichen `16DHBQP040` gefördert.

![Logo BMBF](/images/csm_Logo-BMBF.jpg)

### Projekthintergrund

_Die folgende Beschreibung wurde aus der Projektbeschreibung kopiert._

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
