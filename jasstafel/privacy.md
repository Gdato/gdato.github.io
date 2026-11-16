---
title: "Jass Tafel: privacy policy"
permalink: /jasstafel/privacy
---

# Jass Tafel: privacy policy

Effective date: 16 November 2026  
Publisher: Gdato, Switzerland  
Contact: guillermodato@gmail.com

This policy is for the Android app "Jass Tafel" (package `com.gdato.jasstafel`), as distributed on Google Play and
as the full edition distributed outside Google Play.

## The short version

- **No tracking by us.** No account with us, no analytics, no advertising ID, no crash reporting of our own. We run
  no server, so nothing about you, your phone or your games reaches us.
- **No ads.** There is no advertising code in the app.
- **Everything stays on your phone.** Games, rounds, team names, rule presets and settings are kept in the app's
  private storage, which other apps cannot read. The only way data leaves the phone is when you export or share it
  yourself, or through Android's own app backup if you have that switched on.

One thing comes from Google, not from us, and applies only to the Google Play edition: tips are bought through
Google Play, which handles the purchase under Google's own terms and privacy policy, and the **Google Play Billing
library** that this edition contains may send Google its own technical reports. It is described under "Google Play
Billing".

## What the app stores on your phone

| What | Why | Where |
|---|---|---|
| Games: date, team names, the rules used, every round (trump, points, Weis, Stöck), the winner | The game history and the slate | App database (`jasstafel.db`) |
| Your rule presets | To start a game with your table's house rules | App database |
| Settings: theme, colour palette, text size, keep screen on, vibration, language, slate notation, deck, last team names, and when the tip card was last shown | To remember your choices, and to show the tip card rarely | App storage (`settings`) |
| How many tips this phone has given, and whether one is still being settled (Google Play edition) | To thank you, and to finish a tip that was interrupted | App storage (`support`) |

None of this is personal data unless you type personal names as team names; those stay on your phone like everything else.

## Android backup

Android can back up app data to the Google account on the phone and move it to a new phone. If you have that switched
on, the games, presets and settings above are included (the tip record is not). This is Android's feature under
Google's terms; you can turn it off in Android's settings. The app has no say in it beyond allowing it.

## Export, import and sharing

Settings → Backup writes a JSON file with all your games and presets to a location you choose, and reads such a file
back. The file is yours; the app does not send it anywhere.

"Share result" makes a picture and a short text about a finished game and hands them to the app you choose
(WhatsApp or any other). They go only where you send them.

## Permissions

The full edition has **no internet permission** and declares no permission of its own. The Google Play edition
declares the ones the Google Play Billing library needs (`com.android.vending.BILLING`, `INTERNET`,
`ACCESS_NETWORK_STATE`) and uses the network only through that library; the app's own code opens no network
connection. Neither edition asks for runtime permissions.

## Google Play Billing (Google Play edition only)

Tips are purchases through Google Play, and they unlock nothing: every feature and every colour palette is free for
everyone. Google Play handles the purchase under Google's own terms and privacy policy and holds your payment
details; we never see them, and we receive no personal data through the app. The app on your phone only learns,
through the billing library, that a tip went through, so it can thank you.

The app asks the Google Play app on your phone about purchases each time the app comes to the foreground (to finish a
tip that was interrupted), when you open the support sheet and when you leave a tip.

**The billing library's own reports.** The Play Billing library, written and supplied by Google, is part of the
Google Play edition. It talks to Google Play on the phone, and it includes Google's logging transport (Google
DataTransport), which may send the library's own technical reports to Google, possibly a little later through
Android's job scheduler, also while the app isn't open. The library decides what goes in these reports, not us.
Because the app asks Google Play about purchases each time it comes to the foreground, this may apply to everyone who
uses the Google Play edition, also if you never leave a tip. Google Play services, which the library uses, may also
handle device identifiers and diagnostics of their own. We receive none of this and can't see it. It is covered by
[Google's privacy policy](https://policies.google.com/privacy).

## Full edition (outside Google Play)

The full edition has no billing, no Google code and no internet permission. Its support screen links to an external
donation page, which opens in your browser; what happens on that page is governed by that service's own policy.

## Children

The app is not directed at children under 13. We collect no data from anyone; what Google's billing library may send is
described above.

## Changes

If this policy changes, the new version is published at this address with a new effective date. The app's About
screen links here.
