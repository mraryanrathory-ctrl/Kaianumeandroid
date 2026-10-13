# Kai Anime — Android starter

An original dark/purple Kotlin + Jetpack Compose anime catalogue prototype.

## Implemented in this starter
- Native Android Compose UI
- Search anime metadata using AniList's public GraphQL endpoint
- Anime poster cards and detail screen
- Local watchlist saved in SharedPreferences
- Media3 / ExoPlayer player screen that accepts an HTTPS media URL you are authorized to play

## Important playback limitation
The player is only a playback foundation. No licensed streaming provider has been selected or integrated. Before production, choose a provider that grants your app playback/API rights and implement its official authentication, entitlement checks, stream URL delivery, and DRM requirements. Do not scrape protected streams or hard-code private playback URLs.

AniList supplies catalogue metadata, not video episodes. Review AniList's current API terms and rate limits before public or commercial release:
https://docs.anilist.co/guide/introduction
https://docs.anilist.co/guide/terms-of-use

## Open and run
1. Install Android Studio and its Android SDK.
2. Open this folder as a project in Android Studio.
3. Allow Gradle sync to finish.
4. Run on an Android device or emulator (Android 8.0 / API 26 or later).

This starter does not include the Gradle wrapper files or a compiled APK. Android Studio can create/sync the wrapper for your environment.

## Before release
- Add unit/UI tests and proper loading/error/retry states.
- Persist watch progress and add a Room database.
- Add a provider adapter for a licensed streaming service.
- Handle API usage limits, attribution, privacy, content ratings, accessibility, and store policies.
