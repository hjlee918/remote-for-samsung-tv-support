# Privacy Policy

**Remote for Samsung TV** (Stream Deck plugin), published by Artifex.
Effective date: October 22, 2026.

## Summary

The plugin does not collect, sell, or share personal data. It does not send anything to us or to any server on the internet. Everything it needs stays on your computer and travels only between your computer and your TV on your local network.

## What the plugin stores, and where

The plugin saves the following in Stream Deck's settings on your computer:

- Each TV you paired: its name, model, IP address, network (MAC) address, and its UPnP identifier.
- The token each TV gave the plugin when you allowed it on the TV. It lets your computer control the TV without asking again.
- What you chose for each key or dial, for example "Volume up" or an app to open, and for app keys the app's name and icon, so the key looks right while the TV is off.

This information never leaves your computer except as described below. To delete it, click **Forget** next to a TV in any key's settings, or uninstall the plugin. To also remove the plugin's access on the TV, remove "Stream Deck" from the TV's device list (General → External Device Manager → Device Connection Manager → Device List).

## Network use

The plugin communicates only with TVs on your local network:

- **Search** sends a standard discovery message (SSDP) on your local network to find Samsung TVs, or checks the IP address you enter.
- **Pair**, every key press and every dial turn send commands directly to your TV. While a key or dial is on your Stream Deck, the plugin keeps a connection to the TV open and asks the TV every few seconds whether it's on, its volume, and whether the apps on your keys are on screen, so the keys can show it.
- **Power on** sends a Wake-on-LAN packet on your local network.
- App icons and the list of apps come from your TV.

The plugin makes no connections to the internet. It contains no analytics, tracking, or advertising.

## Logs

Stream Deck keeps a plugin log on your computer to help diagnose problems:

- macOS: `~/Library/Application Support/com.elgato.StreamDeck/Plugins/com.johnlee.samsungtvremote.sdPlugin/logs/`
- Windows: `%APPDATA%\Elgato\StreamDeck\Plugins\com.johnlee.samsungtvremote.sdPlugin\logs\`

The log can include your TV's name and IP address and messages about commands that failed. It does not include the pairing token. The log stays on your computer unless you choose to share it.

## Support requests

If you open an issue in this repository, the issue and anything you attach to it (such as a log) are **public on GitHub** and subject to [GitHub's Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement). Remove anything you don't want to share before posting.

## Purchases

Purchases on the Elgato Marketplace are handled by Elgato (Corsair) and its payment processor, Stripe. We do not receive your payment details. Elgato's privacy policy and [Stripe's Privacy Policy](https://stripe.com/privacy) describe how they handle your data.

## Changes

If this policy changes, the updated version will be posted here with a new effective date.

## Contact

Questions about this policy: [open an issue](https://github.com/hjlee918/remote-for-samsung-tv-support/issues).
