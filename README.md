# Verb Deck

A simple, single-file web app for practicing English irregular verbs. Shuffle through a deck of present-tense verbs, try to recall the past simple and past participle, then reveal the answer to check yourself.

No build step, no dependencies to install — it's one `index.html` file that runs entirely in the browser.

## Features

- 74 common irregular verbs built in (be → was/were → been, go → went → gone, etc.)
- Add your own verbs on the **Word Bank** tab (present, past simple, past participle)
- Check individual verbs in or out of practice, and switch between shuffling the **whole list** or **only checked** verbs
- One button that toggles between "Reveal answer" and "Next word", so it never moves around
- Remembers your custom verbs and checkbox choices in the browser (`localStorage`) between visits
- Works on phones and desktops, and respects light/dark mode

## Running it locally

Just open `index.html` in any browser — no server or build tools required.

## Hosting it for free with GitHub Pages

1. Create a new GitHub repository and push these files to it (see below).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to "Deploy from a branch", pick the `main` branch and the `/ (root)` folder, then save.
4. GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Pushing this folder to GitHub

From inside this folder:

```bash
git init
git add .
git commit -m "Initial commit: Verb Deck"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

(Create the empty repository on GitHub first, then swap in its URL above.)

## Editing the verb list

The built-in verbs live near the top of the `<script>` block in `index.html`, in the `BUILT_IN` array — each entry is `[present, past simple, past participle]`. Add, remove, or edit lines there to change the starter deck.
