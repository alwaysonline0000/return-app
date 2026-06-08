# Return

Return is a static, mobile-first nervous system reset companion for moments of burnout, overwhelm, anxiety, emotional exhaustion, cognitive overload, and difficult life moments.

The product is named `Return` globally and displays `停靠` as its Chinese product title.

Its core experience includes:

- One-tap body reset
- Return Moment reflective questions
- Help and crisis-support pathways
- A personal Safe Kit

The app supports English, Simplified Chinese, Traditional Chinese, and Spanish. All personal content, reset history, and feedback stay in the browser using `localStorage`. There is no backend, account, payment, or analytics integration.

## Run locally

Open `index.html` directly, or serve it locally:

```bash
python3 -m http.server 4173
```

Then open:

```text
http://127.0.0.1:4173/index.html
```

If npm is available, the equivalent command is:

```bash
npm run start
```

## Build

The project is dependency-free and needs no compilation. The build command copies the deployable app into `dist/`:

```bash
npm run build
```

You can also deploy `index.html` directly as a static site.

## Deploy to Vercel

1. Import the repository into Vercel.
2. Keep the included `vercel.json`.
3. Vercel will run `npm run build` and publish `dist/`.

No environment variables are required.

## Deploy to Netlify

1. Import the repository into Netlify.
2. Keep the included `netlify.toml`.
3. Netlify will run `npm run build` and publish `dist/`.

No environment variables are required.

## Local data

The MVP stores these keys in `localStorage`:

- `return-lang`
- `return-kit`
- `return-last-help`
- `return-history`
- `return-feedback`

Clearing browser site data removes these records.

## Product safety

Return is not medical advice or a replacement for professional or emergency support. The Help flow intentionally uses expandable regional support configuration rather than assuming one country.
