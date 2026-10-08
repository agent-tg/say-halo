# Say Halo

This public repository contains notarized Say Halo downloads, release notes, and the signed Sparkle update feed. Application source and private user data are kept elsewhere.

These instructions apply to Say Halo 0.8.14 build 101 and later.

## Download and install

1. Open [Say Halo's latest release](https://github.com/agent-tg/say-halo/releases/latest). Under **Assets**, download the **Say-Halo-0.8.14-build-101.zip** file. The current public download is [0.8.14 build 101 ZIP](https://github.com/agent-tg/say-halo/releases/download/v0.8.14/Say-Halo-0.8.14-build-101.zip). Do not download "Source code." The `say-halo-releases` repository is an archived compatibility feed.
2. Double-click the downloaded ZIP in Finder to extract **Say Halo.app**.
3. Drag **Say Halo.app** into **Applications**, then open it there. Say Halo requires macOS 14 or later.
4. On a new installation, **Setup** opens automatically. Follow its permission, speech model, microphone, shortcut, and clipboard steps.
5. Record a short practice sentence, then test your shortcut in a text field in another app. Return to Setup and confirm that the text appeared. If it did not, copy the transcription from Setup and paste it manually with Command-V, then review Accessibility and clipboard insertion.

Find Say Halo's waveform icon in the menu bar at the top of the screen. Choose **Setup & Troubleshooting...** whenever you need to revisit setup. Advanced preferences remain in **Settings...**.

## If Say Halo will not open

Launch problems happen before in-app Setup can help. If macOS says it cannot verify Say Halo is free of malware, stop and report the exact message, macOS version, download link, and Say Halo version/build to the maintainer. Keep the downloaded file for diagnosis. Do not disable macOS security.

## Setup notes

Allow Microphone for recording, Input Monitoring for the global shortcut, and Accessibility for inserting text in other apps. Setup checks the actual permission status again when you return from System Settings. It does not require Apple's Speech Recognition permission because transcription runs locally.

Model setup can include downloading, compiling, and loading. Download progress applies to the current component and can restart for the next one; it is not an overall model percentage. Preparing may show a spinner without a percentage. Retry after an error; keep existing models.

**Use clipboard to insert** is the recommended setup choice. Say Halo writes the transcription to the clipboard and sends a paste command to the active text field. With **Copy to clipboard** enabled, the transcription stays on the clipboard. Otherwise Say Halo attempts to restore the earlier clipboard after a short delay. Restoration is best effort: a paste command does not prove the other app accepted the text, and slow apps may miss it. Setup always keeps the test transcription available to copy.

## Updating from 0.8.12 or earlier

Versions through 0.8.12 use an update address on the retired `fullstackaiautomation.github.io` host. Install the current release manually once. Version 0.8.13 and later receive updates through the [Sparkle appcast](https://agent-tg.github.io/say-halo/appcast.xml).

If you already have Say Halo installed, quit it before replacing the app in Applications. Your settings and downloaded models stay in place.
