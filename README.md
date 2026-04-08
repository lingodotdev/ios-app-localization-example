# iOS App Localization Example

Demonstrates automated localization for iOS Xcode String Catalogs (`.xcstrings`) using [Lingo.dev](https://lingo.dev) CLI and GitHub Actions.

> **Full walkthrough:** [lingo.dev/en/guides/ios-app-localization](https://lingo.dev/en/guides/ios-app-localization)

## What's inside

- `MyApp/Localizable.xcstrings` - source strings (English)
- `i18n.json` - Lingo.dev CLI configuration
- `.github/workflows/translate.yml` - GitHub Actions workflow

## Quick start

1. Fork this repo
2. Add `LINGODOTDEV_API_KEY` to **Settings > Secrets and variables > Actions**
3. Push a change to source strings in `Localizable.xcstrings`
4. Translations appear automatically via commit to main

## How it works

The Lingo.dev CLI reads the String Catalog, identifies new or changed entries using a lockfile, translates the delta through a configured localization engine, and writes all target languages back into the same `.xcstrings` file. The GitHub Actions workflow runs this on every push to main.

## Locales

- **Source:** `en`
- **Targets:** `es`, `fr`, `de`, `ja`

## Links

- [Guide: iOS App Localization with Xcode String Catalogs](https://lingo.dev/en/guides/ios-app-localization)
- [Lingo.dev CLI docs](https://lingo.dev/en/docs/cli)
- [GitHub Actions integration](https://lingo.dev/en/docs/integrations/github)
- [Create a free account](https://lingo.dev)
