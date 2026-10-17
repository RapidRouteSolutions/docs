# RapidEPR documentation

User guides for [RapidEPR](https://rapidepr.com), built with Mintlify.
The application code lives in
[rapidepr-sst-ion](https://github.com/RapidRouteSolutions/rapidepr-sst-ion).

## Preview and validate

```bash
npx mint dev
npx mint validate
npx mint broken-links
```

`docs.json` controls navigation. Pages use MDX. Internal links start at the
documentation root. Links to the app use `https://rapidepr.com/...`.

## Writing and maintenance

Write for the person using RapidEPR. State prices, features and instructions
directly. Explain what a feature helps them do. Remove retired features,
old navigation names and commentary about how the documentation was reviewed.

Use the [unslop skill](https://github.com/cursor/plugins/blob/main/pstack/skills/unslop/SKILL.md)
when writing public content. Use plain words, sentence case headings and short
sentences. Avoid promotional claims, repeated caveats and unnecessary bold text.

Check navigation against `packages/web/lib/menu-list.ts` and the generator
and settings pages. Check formats against `lib/generator-formats.ts` and the
core format registry. Verify billing and account instructions against their
handlers. Keep release dates tied to the release they describe.

Examples should use the facts supplied in their input. Keep format names as
they appear in the app.

Keep output examples faithful to the selected format. Preserve required citation
openings, closings, capitalization and complete output structure. Apply prose
cleanup to the explanation without replacing a complete citation with an excerpt.
Check examples against their prompt files. Call an example model-generated only
when it comes from an actual recorded generation.
