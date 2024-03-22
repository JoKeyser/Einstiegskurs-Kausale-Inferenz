<!--
SPDX-FileCopyrightText: 2022 Julia Rohrer, Karsten Lübke
SPDX-FileContributor: 2024 Johannes Keyser

SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Einführungskurs Kausale Inferenz

## Beschreibung

Dieses Projekt enthält Materialien für den [KI-Campus-Kurs _Was, wie, warum? - Einführungskurs Kausale Inferenz_](https://ki-campus.org/courses/wwweki) von [Dr. Julia Rohrer](https://juliarohrer.com/) (Universität Leipzig) und [Prof. Dr. Karsten Lübke](https://ki-campus.org/node/793) (FOM Hochschule):

Die enthaltenen Materialien sollen es Lehrkräften erleichtern, das Kursmaterial für den eigenen Unterricht anzupassen.

Wenn Sie das Material studieren wollen, besuchen Sie am besten den originalen Kurs auf [ki-campus.org/courses/wwweki](https://ki-campus.org/courses/wwweki).

Dieses Projekt ist eine Kopie (ein _Fork_) von <https://github.com/luebby/WWWEKI>, mit folgenden (geplanten) Modifikationen:

- (Einige) HTML-Texte werden in Markdown umgewandelt.
- (Einige) Diagramme werden in SVG umgewandelt.
- Die R-Markdown-Dateien (die Grundlage der ShinyApps) werden (auch) in IPython-Notebooks umgewandelt.
- Beispieldatensätze werden als lokale CSV-Dateien bereitgestellt.

Eine genauere Aufschlüsselung der Änderungen finden Sie in Datei [CHANGELOG.md](CHANGELOG.md).

### Was dies nicht ist

Die Lernerfahrung des Kurses auf KI-Campus soll gewährleistet bleiben:
Insbesondere enthält dieses Projekt keine der benoteten Testfragen oder -antworten, da diese im Originalkurs nur unter Zeitdruck zugänglich sind und das Kurszertifikat von ihnen abhängt.


## Installation

Mit [Anaconda](https://anaconda.org/) können Sie alles in einer neuen virtuellen Umgebung mit einem Befehl installieren:

```
conda create --name meinKI jupyter r-irkernel r-tidyverse r-mosaic r-learnr r-ggthemes
```

Um das Material auf GitHub oder GitLab usw. zu betrachten wird nur ein Webbrowser benötigt.

Um die IPython-Notebooks (d.h. die Dateien mit der Endung `.ipynb`) auszuführen oder zu ändern, müssen Sie Jupyter (oder einen geeigneten Editor) installieren.

- FIXME: Testen/Erklärung von Ansatz mit Jupytext!

Sie müssen den `R`-Kernel für Jupyter installieren, um die R-Codezellen ausführen zu können.
Der Kurs stützt sich auf die R-Pakete `tidyverse` und `mosaic`, `learnr`, `ggthemes`, die ihrerseits zusätzliche Abhängigkeiten mit sich bringen.

Optional: Um die Materialien in PDF-Handouts, Folien oder ein anderes Format zu konvertieren, können Sie [Quarto](https://quarto.org/) installieren (das [Pandoc](https://pandoc.org/) enthält, einen leistungsstarken Konverter, den Sie auch ohne Quarto verwenden können).

Optional: Um Ihre Änderungen zu verfolgen und zu diesem Projekt beizutragen, benötigen Sie Git.


## Modulübersicht

1. An der Weggabelung: Einen Weg gehen - und einen nicht (Potential Outcome und Counterfactual)
    - [Externe ShinyApp](https://fomshinyapps.shinyapps.io/WWWEKI_Modul_01/)

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

- Die deutsche Kursvariante auf KI-Campus: <https://ki-campus.org/courses/wwweki>
- Die englische Kursvariante auf KI-Campus: <https://ki-campus.org/courses/whwici>
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

Das Vorhaben *Was, wie, warum? Einstiegskurs Kausale Inferenz (WWWEKI)* wird mit Mitteln des Bundesministeriums für Bildung und Forschung unter dem Förderkennzeichen 16DHBQP040 gefördert.

![Logo BMBF](/images/csm_Logo-BMBF.jpg)
