# GarageLink

GarageLink is a car parts marketplace and community app built with Flutter. It helps drivers search for nearby pickup parts, ship-to-you options, junkyard inventory, and a safe automotive community while also supporting selling parts and managing a garage profile.

## Features

- Nearby pickup search with a 25-mile default radius and up to 100 miles
- Ship-to-you part browsing
- Junkyard listings with location and phone info
- Sell-parts listing workflow
- User garage/build profile
- Community feed for age-appropriate car discussions
- Web-ready Flutter build for browser deployment

## Run locally


## Build for the web


The generated production files are placed in the `build/web` folder and can be hosted on Netlify, Vercel, Firebase Hosting, or any static web host.

## Project status

This is a front-end prototype with sample marketplace data and a polished website-ready experience.

The interface includes a language menu for English, Español, Français, Deutsch, and 日本語. The selected locale updates the app locale and primary navigation; additional marketplace and community copy can be added to `AppStrings` in `lib/main.dart` as translations are reviewed.

## Maintenance

Every pull request and push to `main` or `master` runs formatting checks, `flutter analyze`, the widget tests, and a release web build through GitHub Actions. A scheduled run also checks the project weekly.

Dependabot checks the Dart and GitHub Actions dependencies for updates. Review its pull requests, run the checks locally, and merge updates one at a time so regressions are easy to identify.

To reproduce the CI checks locally:
