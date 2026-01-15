# T-Test - Modell und Realität

![Build PDF](https://github.com/USER/REPO/actions/workflows/build.yml/badge.svg)
![License: MIT](https://img.shields.io/badge/Code%20License-MIT-blue.svg)
![License: CC BY-SA 4.0](https://img.shields.io/badge/Material-CC%20BY--SA%204.0-brightgreen.svg)


Dieses Repository enthält **GeoGebra-Dateien**, **Beamer-Folien** und (optional) **Python-Skripte**  
für Analysis, Stochastik und Vektorrechnung.  
Ziel ist ein moderner Workflow, der Lehrkräften direkt verwendbare Materialien an die Hand gibt und
gleichzeitig einen wissenschaftlich sauberen Entwicklungsprozess sichtbar macht.

---

# 👩‍🏫 1. Für Lehrkräfte (direkte Nutzung)

Wenn Sie einfach mit den Materialien arbeiten möchten, benötigen Sie nur zwei Ordner:

### ✔ `src/GeoGebra/`
GeoGebra-Dateien (`.ggb`) – sofort in GeoGebra Classic 5 oder 6 öffnen.

### ✔ `Folien/`
Beamer-Folien als PDF (und dazugehörige `.tex`-Bausteine).

**Sie müssen keine Programmierung kennen**, um das Material zu verwenden.

---

# 🔍 2. Für Neugierige (Wie ist das gemacht?)

Wenn Sie verstehen möchten, wie die Konstruktionen entwickelt wurden,  
finden Sie hier die wichtigsten Bausteine:

### 📁 Ordnerstruktur (Überblick)

| Ordner | Inhalt |
|-------|--------|
| `src/GeoGebra/` | GeoGebra-Konstruktionen (.ggb) |
| `Folien/`       | modulare Folien (.tex), die von `main.tex` eingebunden werden |
| `fig/`          | automatisch erzeugte Grafiken (PDF/PNG) |
| `tab/`          | Tabellen für Folien |
| `python/`       | Python-Skripte & Notebooks zur Grafikerzeugung |
| `Vorlagen/`     | LaTeX-Stile (`rvmetropolis.sty`), Präambel |

### 🧠 Didaktische Leitidee

GeoGebra wird nicht über Befehlslisten gelernt, sondern über wenige Denkweisen:

1. **Objektorientiert** (Objekte + Eigenschaften)  
2. **Listenorientiert** (Listenoperationen, Folgebefehle)  
3. **Wenige zentrale Befehle** (`Löse`, `Ableitung`, `Ersetze`, …)

Beispiel: Konstruktion eines **Prognoseintervalls** in vier Schritten:

1. Ziel definieren (Diagramm + Randmarkierungen)  
2. Parameter \(n, p, \gamma\) per Schieberegler  
3. Intervallgrenzen mit `ceil`/`floor` und Listen  
4. dynamischer LaTeX-Text (`\text{...}` für normalen Text)

---

# 🧑‍💻 3. Für Profis (kompletter Workflow)

### 📂 Projektstruktur
