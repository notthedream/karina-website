# Karina Website

The English marketing website for Karina Media Player. The macOS app source remains in the separate private `best-media-player` repository. The public `appcast.xml` supplies update information to Karina 7.2.0 and later; release archives must be signed before updating the appcast.

## Publish

GitHub Pages is deployed from the `public/` folder by `.github/workflows/pages.yml` whenever `main` changes.

## Product copy

This page describes features present in Karina Version 7.2. Playback performance, format support, HDR and high-resolution playback vary with the Mac, display and media file. AI subtitle translation is opt-in and sends subtitle text plus nearby dialogue context to the OpenAI API; media files remain on the Mac.

Karina 7.2.0 is available as a universal macOS preview from the public `karina-v7.2.0-preview` release. It requires macOS 15 Sequoia or later and supports Intel and Apple silicon Macs that can run that OS. The preview is not Developer ID signed or notarized, so macOS Gatekeeper may warn or block it on first launch. The website states this limitation; a signed and notarized release requires a Developer ID signing identity.
