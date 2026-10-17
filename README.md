# RapidEPR public documentation

Mintlify user guides for [RapidEPR](https://rapidepr.com). The application source is
[RapidRouteSolutions/rapidepr-sst-ion](https://github.com/RapidRouteSolutions/rapidepr-sst-ion);
this repository does not contain the app or the RapidRegs ingestion service.

## Preview and validate

Use the Mintlify CLI with a supported Node.js version:

```bash
npx mint dev
npx mint validate
npx mint broken-links
```

`docs.json` controls navigation. Pages are MDX; internal page links start at the
documentation root, while app links use `https://rapidepr.com/...`. Do not use
app-relative links such as `/support` inside the docs site.

## Maintenance

Guides were reviewed against app commit `b4f568c` on 2026-10-17. This is a source
alignment date, not a claim about production deployment.

For UI changes, check `packages/web/lib/menu-list.ts`, the generator and settings
routes. Format labels/options come from `lib/generator-formats.ts` and the core
format registry. Check credit/deletion claims against backend behavior, not old
marketing copy. Prices at Stripe checkout are authoritative.

Examples illustrate writing styles; they are not current generated-output
fixtures or guarantees of compliance. Keep historical release entries dated,
and do not invent a release date from the date a guide was edited.
