# Easy Green

Editoriales WordPress-Child-Theme für **Sunflower 26**. Ziel ist eine moderne, barrierearme kommunalpolitische Website mit stark kuratierter Startseite, eigenem redaktionellen Look und sinnvoller Verzahnung mit den Easy-Plugins.

Aktueller Stand: **0.1.11**

## Voraussetzungen

- WordPress 6.7+
- PHP 8.2+
- Parent Theme **Sunflower 26** im Verzeichnis `sunflower26`

## Aktueller Funktionsumfang

- eigener kompakter Header mit Dropdown-Navigation und Sticky/Floating-Zustand
- Sunflower-Social-Profile als gemeinsame Datenquelle
- eigener Footer mit Mitmachen-CTA
- komplett eigene responsive Startseite
- Hero mit frei pflegbaren Headlines, Bild, Text und drei CTAs
- aktuelle Beiträge und dauerhaft kuratierte Themenwelten klar getrennt
- Themenkarten mit Kategorie, festem Bild, eigener Headline und Teaser
- Werkzeuge / Easy-Plugin-Links
- Sunflower-Termine auf der Startseite, falls verfügbar
- Team-Teaser mit vorläufig gepflegten Personenbildern
- Startseiten-Reihenfolge per Drag & Drop
- individuelle Gutenberg-Startseitenblöcke für Text, Bild, Shortcode oder Plugin-Blöcke
- eigenes **Blog-/Aktuelles-Archiv** mit Featured-Beitrag, Themenfilter, Kartenraster und Pagination
- Kategorie-, Schlagwort-, Autoren- und Datumsarchive verwenden denselben editorialen Look

## Einrichtung

1. Sunflower 26 installieren und konfigurieren.
2. Easy Green installieren und aktivieren.
3. Unter **Design → Easy Green** die Startseite konfigurieren.
4. Unter **Design → Startseiten-Blöcke** bei Bedarf freie Sondermodule anlegen.
5. Haupt- und Footer-Menüs wie gewohnt in WordPress zuweisen.
6. Social-Media-Profile weiterhin über die vorhandenen Sunflower-Einstellungen pflegen.

## Versions- und ZIP-Regel

Das Repository enthält die Theme-Dateien direkt im Root. Ein Installations-ZIP muss dagegen **immer exakt einen Theme-Ordner `easy-green/`** enthalten. Der ZIP-Dateiname darf die Versionsnummer tragen.

Richtig:

```text
easy-green-0.1.11.zip
└── easy-green/
    ├── style.css
    ├── functions.php
    └── ...
```

So erkennt WordPress neue Versionen als Update desselben Themes und legt keine doppelten „Easy Green“-Themes an.

Zum lokalen Paketbau:

```bash
./scripts/build-zip.sh
```

Das fertige Paket landet unter `dist/`.

## Nächste sinnvolle Schritte

- Einzelbeitrag im Easy-Green-Look
- normale Inhaltsseite / Landingpage
- Terminarchiv und Termindetail
- Integration von Easy Personen
- später eigene Ratsarbeit / Easy Politics
- Setup-Assistent für neue Ortsverbände

## Changelog

### 0.1.11

- eigenes editorial gestaltetes Blog-/Aktuelles-Archiv
- hervorgehobener neuester Beitrag auf Seite 1
- Themenfilter mit barrierearmen Hover-/Fokuszuständen
- responsive Beitragskarten und Pagination
- Kategorien, Tags, Autoren- und Datumsarchive verwenden dieselbe Gestaltung
- Repository-Workflow vorbereitet und reproduzierbarer ZIP-Build ergänzt

### 0.1.10

- Sunflower-Social-Media-Profile wieder in die Startseite integriert
- Social Icons passen sich dem neuen Header an und verschwinden im Sticky-Zustand
- Theme-Cache-Bereinigung für Altinstallationen aus frühen ZIP-Experimenten

### 0.1.9

- Themenkarten optisch entzerrt: Bild/Headline als starke Karte, längerer Teaser frei darunter
- Verlauf und Bildhöhe für bessere Lesbarkeit der Headline überarbeitet

### 0.1.7–0.1.8

- Backend für aktuelle Beiträge und kuratierte Themenwelten neu strukturiert
- pro Themenwelt festes Bild, Headline und Teaser
- ZIP-Struktur auf stabilen Ordner `easy-green/` korrigiert

### 0.1.1–0.1.6

- Grundlayout, Header/Footer, responsive Startseite, Sticky-Navigation, Themen-/News-Karten, Hover/Fokus-Zustände und erste Backend-Steuerung aufgebaut
