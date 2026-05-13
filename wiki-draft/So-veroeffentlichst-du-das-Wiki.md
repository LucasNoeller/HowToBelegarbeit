# So veröffentlichst du den Entwurf als echtes GitHub-Wiki

Wenn auf der GitHub-Registerkarte **Wiki** nur „Create the first page“ erscheint, ist das normal:

- Ein GitHub-Wiki ist **ein eigenes Git-Repository** (`<repo>.wiki.git`), getrennt vom Haupt-Repo.
- Dateien in `wiki-draft/` erscheinen **nicht automatisch** im Wiki.

## Option A (einfach im Browser)

1. Öffne im GitHub-Repo den Tab **Wiki**.
2. Klicke auf **Create the first page**.
3. Erstelle eine Seite mit dem Titel `Home`.
4. Kopiere den Inhalt aus `wiki-draft/Home.md` hinein und speichere.
5. Lege danach weitere Seiten mit exakt passenden Namen an:
   - `Struktur-einer-Arbeit`
   - `Formalia-und-Formatierung`
   - `Wissenschaftliches-Arbeiten`
   - `Typische-Fehler-und-Checklisten`
   - `Vorlagen-und-Ressourcen`
   - `FAQ`
   - `Glossar`

> Wichtig: Die internen Links funktionieren am besten, wenn die Seitennamen exakt so heißen wie oben.

## Option B (empfohlen: per Git push)

### 1) Wiki-Repo klonen

```bash
git clone https://github.com/<OWNER>/<REPO>.wiki.git
cd <REPO>.wiki
```

### 2) Entwurf aus dem Haupt-Repo kopieren

```bash
cp -v ../<REPO>/wiki-draft/*.md .
```

### 3) Commit & Push

```bash
git add .
git commit -m "Initial wiki content"
git push
```

Danach sollte der Tab **Wiki** die Seiten sofort anzeigen.

## Typische Stolperfallen

- **Wiki deaktiviert:** In den Repo-Settings muss „Wikis“ aktiviert sein.
- **Falscher Dateiname der Startseite:** `Home.md` muss vorhanden sein.
- **Schreibrechte fehlen:** Du brauchst Push-Rechte auf das Repository.
