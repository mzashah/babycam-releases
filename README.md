# BabyCam — releases & landing page

This small **public** repo holds BabyCam's public-facing pieces — it contains **no app source code**
(the app source is in a separate private repo).

- **Landing page:** [`index.html`](index.html) → served at **https://mzashah.github.io/babycam-releases/**
- **Release assets:** each GitHub Release here carries two fixed-name files the app depends on:
  - `app-release.apk` — the installable app
  - `version.json` — `{ "versionCode", "versionName", "mandatory", "notes" }`, read by the app's
    in-app updater and by the landing page to show the latest version.

The "Download APK" buttons on the landing page point at
`releases/latest/download/app-release.apk`, so publishing a newer release automatically updates both
the site and every installed app's update check.
