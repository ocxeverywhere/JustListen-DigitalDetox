# Plan: Update website for Firebase telemetry

## Context

Update the Korean and English home pages and the bilingual privacy-policy page so the public site matches the Firebase-enabled Android release. Remove obsolete summary/Gemini product claims, document the active caption-to-speech flow and Android share entry point, and replace inaccurate no-collection claims with cautious Firebase disclosures. Use July 19, 2026 as the publication/effective/last-updated date unless the operator supplies another date before implementation.

## Approach

Revise only the existing static HTML pages, preserving their current layout, navigation, local-library claims, and background-playback claims. Keep Korean and English product copy equivalent. In the policy, replace Gemini-specific processing with the active optional translation, rule-based cleanup, and project Cloud TTS flow; add Firebase Analytics, Crashlytics, Performance Monitoring, and Remote Config sections; distinguish custom telemetry exclusions from Firebase SDK technical processing; document local activation/review counters; and separate device-local deletion from Firebase-managed retention and privacy requests. Avoid unconfirmed promises about consent, legal basis, retention periods, international transfers, and Google Play collected/shared classifications.

## Files to modify

- `C:\PrivateProject\JustListen-DigitalDetox\index.html` — update Korean metadata, hero/product/features, Android sharing note, store date, and Firebase data-safety wording.
- `C:\PrivateProject\JustListen-DigitalDetox\en\index.html` — apply the equivalent English homepage and listing changes.
- `C:\PrivateProject\JustListen-DigitalDetox\privacy\index.html` — update Korean policy and English summary with current processing, Firebase categories/boundaries, local-state retention/deletion distinctions, service links, contact guidance, and dates.

## Reused code

- `C:\PrivateProject\JustListen-DigitalDetox\index.html:487` — retain the existing static feature-grid structure for revised product and sharing copy.
- `C:\PrivateProject\JustListen-DigitalDetox\index.html:501` — retain the existing definition-list structure for store details and data-safety wording.
- `C:\PrivateProject\JustListen-DigitalDetox\privacy\index.html:318` — reuse the responsive policy table structure for expanded data categories.
- `C:\PrivateProject\JustListen-DigitalDetox\privacy\index.html:400` — reuse the existing numbered third-party-service section structure for Firebase services.
- `C:\PrivateProject\JustListen-DigitalDetox\privacy\index.html:503` — retain the existing `#english` route so current English navigation remains valid.

## Language(s) detected

mixed: html, css

## Verification

- Search all three HTML files for obsolete live claims: `Gemini`, `summary`, `summaries`, `요약`, and the exact no-data-safety phrases; confirm none remain in product/policy claims.
- Confirm both home pages describe URL entry, caption fetching, optional translation, rule-based cleanup, Cloud TTS, local sessions, background playback, and Android text sharing consistently.
- Confirm the policy names all four Firebase services, all required data categories, SDK technical-data caveat, custom telemetry exclusions, local review counters, and local-versus-Firebase deletion/retention boundaries in both languages.
- Validate internal links and anchors, especially `en/`, `privacy/`, and `privacy/#english`, and confirm Korean/English dates match.
- Parse the HTML with an available validator or browser, then inspect desktop and narrow mobile layouts for tables, cards, navigation, and policy readability.
- Review the final diff to ensure business identity, Google Play URL, app ID, contact email, local-library wording, and background-playback wording were not unintentionally changed.
