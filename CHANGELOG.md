# Changelog - Änderungsverlauf

Diese Datei enthält eine Zusammenfassung der Änderungen relativ zum [Upstream-Projekt](https://github.com/luebby/WWWEKI).
Die exakten Änderungen sind den jeweiligen Git-Commits zu entnehmen.

- Anpassen der Projkektinformationen in [README.md](README.md).
- Text der Lizenz CC-BY-SA-4.0 in [LICENSE.txt](LICENSE.txt) gespeichtert.
- Kosmetik: Pro Satz eine eigene Zeile im Markdown.
- Kosmetik: Externe URLs per `<URL>` markieren statt wiederholung mit `[URL](URL)`.
- Kosmetik: Inline Code-Ausgabe (`r ...`) in Markdown-Zellen verschieben oder löschen.
    - NOTE: Ggf. funktioniert das aber mit neueren JupyterLab-Versionen?
- Für Anpassung an Jupyter: Inkompatible Verwendung von R-Code in LaTeX-Gleichungen umgehen.
- Für PDF-Export: Konversion von HTML-Farben in LaTeX-Farben, z. B. `<blue>Gehalt</blue>` -> `$\color{blue}\text{Gehalt}$`
- Für PDF-Export: Anpassung von LaTeX-Formeln ohne inhaltliche Änderungen:
    - Tauschen von Hoch- und Niedrigstellung (mit `^{}` und `_{}`).
    - Farbwechsel von `color{green}` (sehr hell) zu `color{DarkGreen}` (dunkler) für bessere Lesbarkeit und Ähnlichkeit zum KI-Kurs-HTML.
    - Begrenzung der Farbanwendung mithilfe zusätzlicher Gruppierung (mit `{}`).
- Erwähnung des Löschens von [KI-Campus](https://ki-campus.org/) in README und Löschen der "toten" Links auf KI-Campus.
- ...

