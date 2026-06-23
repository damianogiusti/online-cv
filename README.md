# online-cv

Damiano Giusti's résumé — a single static page built from `_data/data.yml` by a
tiny Node generator (`build.mjs`). No Jekyll, no framework. Shares the
[blog](https://www.damianogiusti.com) theme (`style.css`): monospace, minimal,
light/dark following the OS with a persisted toggle.

## Edit

All content lives in **`_data/data.yml`** — profile, experience, projects,
education, skills. Change it there and rebuild.

## Develop

```sh
npm install
node build.mjs          # -> dist/
npx serve dist
```

Deployed to GitHub Pages via `.github/workflows/deploy.yml`; served under
`/online-cv` (the `BASE` constant in `build.mjs`).
