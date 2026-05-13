# Formalia & Formatierung

## Empfohlene Grundeinstellungen

| Element | Empfehlung (Beispiel) |
|---|---|
| Schrift | 11–12 pt (z. B. Times/Arial) |
| Zeilenabstand | 1.5 |
| Seitenränder | 2.5 cm |
| Blocksatz | Ja, mit Silbentrennung |
| Seitenzahlen | Ab Einleitung sichtbar |

> Beachte immer die Vorgaben deiner Hochschule – diese haben Vorrang.

## Überschriften-Hierarchie

- H1: Kapitel
- H2: Unterkapitel
- H3: Unter-Unterkapitel

Nicht tiefer als H3/H4 gliedern (Lesbarkeit!).

## Zitation: Gute Praxis

- Direktzitat: mit Seitenzahl
- Indirektes Zitat: Quelle dennoch nennen
- Einheitliche Schreibweise im ganzen Dokument

### LaTeX-Beispiel

```tex
\documentclass[12pt,a4paper]{article}
\usepackage[ngerman]{babel}
\usepackage[T1]{fontenc}
\usepackage{csquotes}
\usepackage[backend=biber,style=apa]{biblatex}
\addbibresource{literatur.bib}
```

### Word-Tipp

Nutze **Formatvorlagen** statt manueller Schriftänderungen – so bleiben Inhaltsverzeichnis und Nummerierungen stabil.
