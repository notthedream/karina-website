# Karina Website

The English marketing website for Karina Media Player. The macOS app source remains in the separate private `best-media-player` repository. The public `appcast.xml` supplies update information to Karina 7.2.0 and later; release archives must be signed before updating the appcast.

## Publish

GitHub Pages is deployed from the `public/` folder by `.github/workflows/pages.yml` whenever `main` changes.

## Product copy

This page describes features present in Karina Version 7.2. Playback performance, format support, HDR and high-resolution playback vary with the Mac, display and media file. AI subtitle translation is opt-in and sends subtitle text plus nearby dialogue context to the OpenAI API; media files remain on the Mac.

Karina 7.2.0 is available as a universal macOS preview from the public `karina-v7.2.0-preview` release. It requires macOS 15 Sequoia or later and supports Intel and Apple silicon Macs that can run that OS. The preview is not Developer ID signed or notarized, so macOS Gatekeeper may warn or block it on first launch. The website states this limitation; a signed and notarized release requires a Developer ID signing identity.

## Future app updates

Keep the Sparkle Ed25519 private signing key in the macOS login Keychain under account `karina-media-player`; do not commit the private key. For each new app release, increment the app's bundle version, create the ZIP, sign it with Sparkle's `sign_update --account karina-media-player <archive>`, upload the archive, and update the version, download URL, length and public signature in `public/appcast.xml` before publishing the site. Versions 7.0 and 7.1 need a manual install of 7.2 before they can receive automatic update prompts.
