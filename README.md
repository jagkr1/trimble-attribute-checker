# Trimble Connect Attribute Checker

First version: checks selected objects against `rules.json`.

## Files

- `index.html` - the extension
- `manifest.json` - manifest for project-level extension installation
- `rules.json` - project-specific rules exported from Attribute Rule Builder

## GitHub Pages setup

1. Create a new GitHub repository.
2. Upload these three files to the root of the repository.
3. Open repository Settings > Pages.
4. Set Source to `Deploy from a branch`.
5. Select branch `main` and folder `/root`.
6. Save.

Your URLs will look like:

- `https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/index.html?v=1`
- `https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/manifest.json?v=1`
- `https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/rules.json?v=1`

## Important

Edit `manifest.json` and replace:

`https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/index.html?v=1`

with your real GitHub Pages index URL.

## Trimble Connect setup

In Trimble Connect for Browser, install the custom extension using the manifest URL:

`https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/manifest.json?v=1`

For the 3D viewer custom extension workflow, you may need to add the plugin URL directly instead:

`https://YOUR-GITHUB-USERNAME.github.io/YOUR-REPOSITORY-NAME/index.html?v=1`

## First test

1. Open a model in the 3D viewer.
2. Select one object.
3. Open the Attribute Checker extension.
4. Press `Load rules`.
5. Choose a rule set.
6. Press `Inspect selected object`.
7. Check whether the property paths match your `rules.json`.
8. Press `Check selected objects`.
