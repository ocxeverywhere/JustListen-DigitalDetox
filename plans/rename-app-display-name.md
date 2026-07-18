# Plan: Rename the public app display name

## Context

The public app name changed from `JustListen - Digital Detox` to `JustListen: 유튜브를 팟캐스트로` in Korean and `JustListen: Youtube as Podcast` in English. Update the static website so formal app-name references match the store name while preserving the short `JustListen` brand in ordinary prose and compact navigation.

## Approach

Replace formal display-name occurrences in page titles, metadata, hero introductions, store-detail app-name fields, privacy-policy titles, policy app-name fields, image labels, and formal privacy-policy references. Keep `JustListen` as the short brand in navigation, explanatory prose, Android Settings instructions, copyright text, URLs, email addresses, package ID, and asset paths. Use the exact English spelling supplied by the operator: `Youtube`.

## Files to modify

- `C:\PrivateProject\JustListen-DigitalDetox\index.html` — apply the new Korean display name to formal homepage metadata, hero/store copy, and accessible labels.
- `C:\PrivateProject\JustListen-DigitalDetox\en\index.html` — apply the new English display name to the equivalent formal references.
- `C:\PrivateProject\JustListen-DigitalDetox\privacy\index.html` — update Korean policy and English summary titles, metadata, and formal app-name fields while retaining short-brand prose where appropriate.

## Reused code

- Existing title, metadata, store-detail, and privacy-policy structures remain unchanged; this is a copy-only update.

## Language(s) detected

html

## Verification

- Search all three HTML files and confirm `JustListen - Digital Detox` no longer appears.
- Confirm the Korean formal name is used only on Korean-facing formal labels and the English formal name only on English-facing formal labels.
- Confirm package ID, Google Play URL, asset paths, email address, language links, and `privacy/#english` remain unchanged.
- Run `git diff --check` and inspect the diff for copy-only changes.
