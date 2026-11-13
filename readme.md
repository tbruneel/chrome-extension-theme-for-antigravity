# Title Bar Theme for Google Antigravity

A lightweight, zero-configuration Chrome extension that matches the window title bar and startup screen of the **Google Antigravity** desktop app in Chrome to your active color theme.

## What Is This Project?

When you install and run [Google Antigravity](https://antigravity.google.com/) as a standalone Chrome app on Windows, it opens in its own dedicated window with a native desktop title bar across the top. This extension automatically keeps that window title bar and the app's launch screen in sync with the colors inside the Antigravity workspace.

## Why Does It Exist?

By default, Google Antigravity instructs Chrome to display a fixed dark-gray title bar at all times—even when you switch to Light mode, turn on Strong Contrast, choose a custom color in **Settings → Appearance**, or open a dimmed pop-up window such as Settings. That mismatch leaves a contrasting bar stuck across the top of your screen and causes a dark-gray flash when launching the app.

This extension solves that automatically with zero settings to manage:

- Matches Light mode, Dark mode, Default Contrast, Strong Contrast, and custom Appearance themes.
- Dims smoothly in real time whenever Settings, drawers, or pop-up dialogs open and restores immediately when they close.
- Remembers your base theme color locally so launching the app opens with a matching startup screen instead of flashing an unmatched color.

> [!NOTE]
> Window title bar coloring applies to **standalone Chrome app windows** (created via Chrome's **menu (`⋮`) → Cast, save, and share → Install page as app…**). Regular Chrome browser tabs use Chrome's normal tab strip and are unaffected.

## Installation

### Option 1: Chrome Web Store (Recommended)

1. Open the extension listing on the Chrome Web Store: [Title Bar Theme for Google Antigravity](https://chromewebstore.google.com/detail/gffpamdcddmdbeljekjlpaknpmjlglni).
2. Click **Add to Chrome**.
3. Open the Google Antigravity Chrome app—your title bar updates automatically with no further setup.

### Option 2: Chrome Developer Mode (Local Setup)

1. Clone or download this repository to a folder on your computer.
2. Open Google Chrome and go to `chrome://extensions/`.
3. Turn on **Developer mode** using the toggle in the top-right corner.
4. Click **Load unpacked** in the top-left and select the root folder of this repository (the folder containing `manifest.json`).
5. Open **Google Antigravity** (`https://antigravity.google.com/`) in its standalone Chrome app window.

## Documentation

- [**Technical Documentation**](./docs/technical.md) — Architecture, implementation details, and design rationale.
- [**Privacy Policy**](./docs/privacy.md) — Privacy details (zero data collection; all theme detection runs locally in your browser).
