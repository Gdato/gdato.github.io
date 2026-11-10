---
title: "Jass Tafel: privacy policy"
permalink: /jasstafel/privacy
---

# Jass Tafel: privacy policy

Effective date: 9 November 2026  
Publisher: Gdato, Switzerland  
Contact: guillermodato@gmail.com

This policy is for the Android app "Jass Tafel" (package `com.gdato.jasstafel`), as distributed on Google Play and
as the full edition distributed outside Google Play.

## The short version

- **The app collects nothing.** No account, no analytics, no advertising identifier, no crash reporting. We run no
  server, so nothing about you, your phone or your games reaches us.
- **No ads.** There is no advertising code in the app.
- **Everything stays on your phone.** Games, rounds, team names, rule presets and settings are kept in the app's
  private storage, which other apps cannot read. The only way data leaves the phone is when you export it yourself,
  or through Android's own app backup if you have that switched on.

The one thing you should know about comes from Google, not from us: the **Google Play Billing library**, which apps
that sell through Google Play must build in, is part of the Google Play edition. It is described below.

## What the app stores on your phone

| What | Why | Where |
|---|---|---|
| Games: date, team names, the rules used, every round (trump, points, Weis, Stöck), the winner | The game history and the slate | App database (`jasstafel.db`) |
| Your rule presets | To start a game with your table's house rules | App database |
| Settings: theme, colour palette, large text, keep screen on, vibration, language, slate notation, deck, last team names | To remember your choices | App storage (`settings`) |
| Whether you are a supporter (Google Play edition) | So the supporter palettes work offline | App storage (`support`) |

None of this is personal data unless you type personal names as team names; those stay on your phone like everything else.

## Android backup

Android can back up app data to the Google account on the phone and move it to a new phone. If you have that switched
on, the games, presets and settings above are included. This is Android's feature under Google's terms; you can turn
it off in Android's settings. The app has no say in it beyond allowing it.

## Export and import

Settings → Backup writes a JSON file with all your games and presets to a location you choose, and reads such a file
back. The file is yours; the app does not send it anywhere.

## Permissions

The full edition declares **no permissions**. The Google Play edition declares the ones the Google Play Billing
library brings with it (`com.android.vending.BILLING`, `INTERNET`, `ACCESS_NETWORK_STATE`); the app itself opens no
network connection. Neither edition asks for runtime permissions.

## Google Play Billing (Google Play edition only)

Tips and the one-time supporter unlock are purchases through Google Play. Google processes the payment and holds your
payment details; we never see them. We only learn, through the billing library, that a purchase happened, so the app
can thank you and, for the supporter unlock, remember it on your phone.

The billing library is Google's code running inside the app. It talks to Google Play on the phone and may send
Google technical information about the app and the purchase, as described in
[Google's privacy policy](https://policies.google.com/privacy). We receive none of it. Purchases can be
restored on another phone signed in to the same Google account (Settings → Support → Restore purchases).

## Full edition (outside Google Play)

The full edition contains no Google code. Its support screen links to an external donation page in your browser;
what happens on that page is governed by that service's own policy.

## Children

The app is not directed at children under 13 and collects no data from anyone.

## Changes

If this policy changes, the new version is published at this address with a new effective date. The app's About
screen links here.
