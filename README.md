# vireal.dev

Static Astro site for `https://vireal.dev`.

## Local development

```bash
npm install
npm run dev
```

## Production build

```bash
npm run build
```

Astro writes the static site to `dist/`.

## Cloudflare Pages

Recommended setup:

- Framework preset: **Astro**
- Build command: `npm run build`
- Build output directory: `dist`
- Production branch: `main`
- Custom domain: `vireal.dev`

Expected public routes:

- `/`
- `/projects/`
- `/vmtr01/`
- `/vmtr01/privacy/`
- `/vmtr01/terms/`
- `/vmtr01/support/`

## Before VMTR01 store submission

The privacy page is an initial draft based on the intended Amplitude telemetry model. Before publishing the app:

1. verify the actual Amplitude payloads sent by the production build;
2. ensure disabled fields (IP-derived geo, advertising ID, App Set ID, carrier, etc.) are not transmitted;
3. update the policy if the final event/property schema differs;
4. add a stable support/privacy contact address;
5. make Google Play Data Safety declarations match the implementation and policy.
