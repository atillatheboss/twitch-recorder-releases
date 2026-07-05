# Twitch Recorder iOS Releases

[🇩🇪 Deutsche README](README.de.md)

This repository contains public release builds and an AltStore-compatible source for **Twitch Recorder iOS**.

Twitch Recorder iOS can be opened and used locally on your iPhone without connecting to the recorder server first. The app includes the local recording and media areas, settings, playback-related features, and the full in-app experience even when no server is configured.

For the best experience and for reliable real AFK recordings, you should also install and run the Twitch Recorder server. The server can keep recording in the background on another device, so your iPhone does not have to stay open, unlocked, or connected the whole time.

## AltStore Source

You can install Twitch Recorder iOS through the AltStore-compatible source from this repository.

Source URL:

```txt
https://raw.githubusercontent.com/atillatheboss/twitch-recorder-ios-releases/main/altstore-source.json
```

The AltStore source is generated automatically from the latest release. When a new release is published, the source will be updated so compatible apps can detect the newest version.

## How It Works

Twitch Recorder iOS can be used as a standalone local app or as a companion app for the Twitch Recorder server.

You do not need to connect a server just to start and use the app. The recordings, media views, local settings, and general app functionality are available directly inside the iOS app.

For proper unattended recording workflows, the recorder server is recommended. The server handles long-running recording, downloading, processing, and media management outside of the iPhone. This is especially useful when you want recordings to continue while you are away.

You can use the app in two ways:

### Local App Mode

Use the app without connecting to a server.

This gives you the full local app experience, including:

- Opening and using the app without server setup
- Accessing the recordings and media sections in the app
- Using local playback and media-related app features
- Managing app settings
- Preparing the app before connecting it to a recorder server later

### Server Mode

Connect the app to a running Twitch Recorder server.

This is recommended for the best experience and for real AFK recording workflows:

- Start Twitch recordings that run on the server
- Schedule recordings
- Let recordings continue without actively using your iPhone
- Manage active and scheduled jobs
- Browse recordings created by the server
- Play recorded media
- Search and download VODs and clips
- View recorder metrics and server settings

For casual app usage, Local App Mode is enough. For reliable unattended Twitch recordings, Server Mode is recommended.

## Automatic Server Detection

The app can automatically detect a compatible recorder server on your network.

To use this:

1. Start the Twitch Recorder server on your Mac, NAS, home server, or Docker host.
2. Make sure your iPhone is on the same network or connected through VPN.
3. Open the app.
4. Tap **Configure Recorder Server**.
5. Select the detected server or enter the server manually if needed.

## Features

- Use the app locally without setting up the server first
- Access the recordings and media areas directly inside the app
- Use the full local app experience without a recorder server
- Automatically detect the recorder server from the app
- Start Twitch recordings from your iPhone when connected to a server
- Select stream quality, schedule, duration, end time, and chat options
- Search Twitch channels with live/offline status
- Manage active and scheduled recording jobs
- Pause, resume, stop, cancel, and extend jobs
- Browse recorded media
- Copy recording links
- Finalize MP4 recordings
- Play recordings natively on iOS
- Search and download Twitch VODs and clips through the server
- Manage download jobs and downloaded media
- View recorder metrics and app/server settings

## Requirements

To use the app locally, you need:

- An iPhone
- A valid IPA build or the AltStore-compatible source
- A sideloading method such as LiveContainer, SideStore, or AltStore

For the best AFK recording experience, you also need:

- A running Twitch Recorder server
- Network access from the iPhone to the server
- Enough storage on the server host for recordings

## Installation

You can install the app through the AltStore-compatible source or by manually installing the IPA.

### Option 1: Install Through the AltStore Source

1. Install **LiveContainer**, **SideStore**, or **AltStore** on your iPhone.
2. Open the app you want to use for sideloading.
3. Go to the **Sources** section.
4. Add the source URL from this README.
5. Find **Twitch Recorder iOS** in the source.
6. Install the app.
7. Open Twitch Recorder iOS.
8. Use it locally or tap **Configure Recorder Server** to connect to your recorder server.

### Option 2: Install the IPA Manually

1. Open the [Releases](https://github.com/atillatheboss/twitch-recorder-ios-releases/releases) page.
2. Download the latest IPA file.
3. Open LiveContainer, SideStore, or AltStore.
4. Import or install the downloaded IPA.
5. Open Twitch Recorder iOS.
6. Use it locally or configure the recorder server for AFK recording features.

## LiveContainer Status

The app has currently only been tested with **LiveContainer**.

SideStore and AltStore installation should work in principle through the same IPA or AltStore source workflow, but they have not been tested yet.

Tested:

- LiveContainer

Not tested yet:

- SideStore
- AltStore

## Recommended Setup

You can use the app completely locally on your iPhone.

For the best AFK recording setup:

1. Install the iOS app through LiveContainer.
2. Start the Twitch Recorder server on a device that stays online.
3. Open the app.
4. Tap **Configure Recorder Server**.
5. Let the app detect the server automatically.
6. Start and manage your recordings from your iPhone.

This setup allows recordings to continue even when you are not actively using your iPhone.

## Playback

Native iOS playback is implemented through an `AVPlayerViewController` bridge. No additional Flutter video plugin is required for playback.

## Notes

- The app can be opened and used without the recorder server.
- The recordings and media areas are available inside the app without connecting a server.
- The full local app experience is available directly on the iPhone.
- For reliable AFK recordings, the Twitch Recorder server is recommended.
- The server performs long-running recording, downloading, processing, Streamlink, and FFmpeg tasks.
- The iOS app acts as a local interface, remote control, and media browser.
- Make sure your iPhone and server can reach each other over the same network or through VPN when using Server Mode.
- The AltStore source is updated automatically from the latest release.

## Disclaimer

This project is not affiliated with, endorsed by, or sponsored by Twitch. Use it responsibly and follow Twitch’s Terms of Service and applicable laws.
