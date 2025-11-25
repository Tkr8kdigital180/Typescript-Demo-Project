# TypeScript DevOps Übungsprojekt

Dieses Projekt wurde entwickelt, um DevOps-Workflows mit npm, Jenkins und GitHub Actions zu üben.

## Erste Schritte

1.  Repository klonen:
    ```bash
    git clone https://github.com/StephanLoecher/Typescript-Demo-Project.git
    cd Typescript-Demo-Project
    ```
2.  Abhängigkeiten installieren:
    ```bash
    npm install
    ```
3.  Projekt bauen:
    ```bash
    npm run build
    ```
4.  Tests ausführen:
    ```bash
    npm test
    ```

## CI/CD Übungen

1.  **Jenkins**: Erstellen Sie ein `Jenkinsfile`, das eine Pipeline mit den folgenden Stufen definiert:
    -   Install (Installieren)
    -   Build (Bauen)
    -   Test (Testen)
    -   Audit (Prüfen)
2.  **GitHub Actions**: Erstellen Sie eine `.github/workflows/ci.yml` Datei, die bei Push und Pull Requests auf `main` ausgelöst wird und die gleichen Schritte wie oben ausführt.

> **Wichtig**: Vergessen Sie nicht, den Workspace im `post`-Abschnitt der Jenkins-Pipeline zu bereinigen!

## Übungen

Siehe `exercises/AUDIT_UPDATE.md` für Anweisungen zum Üben von Paket-Audits und -Updates.

## Abgabe

- Branch erstellen: `exercise/ci-audit-<INITIALEN>`
- Dateien einfügen:
  - `Jenkinsfile`
  - `ci.yml`
  - Dokumentation / Screenshots
  - Reflektion
- Pull Request gegen `main` erstellen.
