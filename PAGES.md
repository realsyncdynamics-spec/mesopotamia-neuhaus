# GitHub Pages einmalig einschalten

Der Workflow `Deploy Pages` existiert und läuft bei jedem Push auf `main`.
Er kann die Site **nicht selbst anlegen**. Fehler bisher:

`Create Pages site failed. Resource not accessible by integration`

## Pflichtklick (Kontoinhaber)

1. https://github.com/realsyncdynamics-spec/mesopotamia-neuhaus/settings/pages
2. **Build and deployment → Source:** `GitHub Actions`
3. Speichern.
4. Danach: https://github.com/realsyncdynamics-spec/mesopotamia-neuhaus/actions/workflows/pages.yml → **Run workflow** → Branch `main`.

## Alternative ohne Actions

Dieselbe Settings-Seite:

1. Source: **Deploy from a branch**
2. Branch: `main`
3. Folder: `/ (root)`
4. Save

Dann liegt die Site unter:
https://realsyncdynamics-spec.github.io/mesopotamia-neuhaus/

Repo muss öffentlich sein oder das Konto braucht GitHub Pages für private Repos.
