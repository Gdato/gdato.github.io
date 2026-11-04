---
title: "Universal Remote: privacy policy"
permalink: /universal-remote/privacy
---

# Universal Remote: privacy policy

Effective date: 4 November 2026  
Publisher: Gdato, Switzerland  
Contact: guillermodato@gmail.com

This policy is for the Android app "Universal Remote & Diagnostics" (package `com.gdato.universalremote`) as
distributed on Google Play. It goes with the [terms of use](terms.md).

## The short version

- **No tracking.** No account with us, no analytics, no advertising ID, no crash reporting. We have no server, so we receive
  nothing about you, your phone or your devices.
- **No ads.** Not in the free version, not in Pro. There is no advertising code in the app.
- **No hidden processes.** The app talks only to the devices you choose, on your Wi-Fi or over Bluetooth, and to
  Google Play for the Pro purchase. We wrote no background service, scheduled task or start-with-the-phone code.
  When you leave the app, its scans, status refreshes, live views and keep-alive connections pause; a job you sent to a
  device (cleaning, mowing, opening a gate) is finished by the device, and a file you cast stays available while it
  plays, for up to 30 minutes.

There is one exception you should know about, and it comes from Google, not from us: the **Google Play Billing
library**, which apps that sell through Google Play build in. It sends Google its own technical reports, described
below. We never see them.

## What stays on your phone

Everything the app knows is kept in its private storage on your phone, which other apps can't read:

| What | Why | Where |
|---|---|---|
| Your saved devices: names, addresses, presets, settings, and the passwords, keys or tokens you enter for them | To connect to those devices again | App storage (`profiles`) |
| App settings (developer mode, quiet discovery, that you accepted the first-run notice) | To remember your choices | App storage (`settings`) |
| Whether you own Pro | So Pro works offline | App storage (`pro`) |
| Fingerprints of the security certificates your TVs, speakers and hubs use | To refuse a different machine pretending to be your device. A changed certificate is always refused; to accept it, forget the device and add it again | App storage (`tls_pins`) |
| Which home-screen widget opens which saved device (Pro) | So each widget opens the right device | App storage (`widgets`) |
| The phone's own Bluetooth name, only if an earlier version's Quiet discovery masked it and a pairing was interrupted | So the app can put the name back at its next start; the entry is then deleted | App storage (`incognito`) |
| Pairing keys for Android TV and network debugging (ADB) | So a TV or box you paired accepts the phone again | Android Keystore, which doesn't let the key leave the phone |
| Temporary files: a spoken announcement or a file you send to a speaker or TV | To serve it to that device. While it plays, a cast file is served by a small temporary server in the app at a random address on your home network, which other devices on that network could also reach. Only one such server runs at a time: casting the next file stops the previous one. It stops after 30 minutes at most, and the copied file is then deleted | App cache; Android may clear it at any time |

Scan results exist only while the app is open. The app doesn't use your location, contacts, photos or files, except a
file you pick yourself.

**Android's own backup.** If you have turned on backup to your Google account in Android's settings, Android may copy
only the app's settings (`settings`: theme and developer options, and that you accepted the first-run notice) into that
backup. Your saved devices with their logins, keys and tokens, the certificate fingerprints, the widget list, the
`incognito` entry and the Pro flag are all excluded from Google backup and from phone-to-phone transfer. Pro is restored
from Google Play instead ("Restore purchase").

**Files you create.** With Pro you can save a backup of your devices. It is encrypted with a password you choose, at least 10
characters (AES-256-GCM, key derived with PBKDF2 at 600,000 iterations), and it goes only where you save it. Car or machine recordings (CSV) are also
saved only where you choose. If you save either to a cloud folder, that service's own privacy terms apply.

**Home-screen shortcuts and widgets** (Pro) store the device's name and an internal reference with your launcher. A widget only opens the app on that device: it never contacts the device and runs on no schedule.

**Diagnostics log.** Only in developer mode, the app writes technical events (event names, device addresses, timings,
error codes; never passwords, keys or tokens) to Android's system log on the phone. It is never uploaded. It can be
read only from a computer connected by USB with debugging turned on.

## What leaves your home network

Normally, nothing: the app talks directly to your devices over Bluetooth or on your local network. These are the only
exceptions in the Google Play version.

### 1. Google Play, for the Pro purchase

Only when you open a Pro feature or the Pro page, buy, or tap "Restore purchase", the app asks the Google Play app on your phone whether your Google account owns Pro and what it costs. If you
own Pro, the app also confirms the purchase about once a week when it starts, so a refunded purchase doesn't stay
unlocked. The Pro page opens from Settings, when you reach the free limit of 2 devices, and when you tap a Pro feature as a
free user: the developer-mode switch, backup and restore, home-screen shortcuts and widgets, and the Pro locks on the
camera, dashcam and car-diagnostics screens. If you use the free version and never open a Pro feature or the Pro page,
the app doesn't contact Google Play at all. When you buy, Google Play shows its own
payment screen. Google Play then talks to Google using your Google account. What Google receives from the app: its
package name, the product (`pro_unlock`) and, after a purchase, a confirmation for that purchase (so Google doesn't
refund it automatically). We never receive your name, email address or payment details.

### 2. Google Play Billing library reports

The Play Billing library, written and supplied by Google, is part of the app. It sends technical reports about its own
work (for example which billing step ran and its result, and the library version) to Google's logging service at
`firebaselogging.googleapis.com` and `firebaselogging-pa.googleapis.com`. The library decides what goes in these
reports, not us. It uses Android's job scheduler, so a report may be sent a little later, also while the app isn't
open. This happens only when the app talks to Google Play (see above), never for a free user who doesn't open a Pro
feature or the Pro page. We don't receive these reports and can't see them.

Both are covered by [Google's privacy policy](https://policies.google.com/privacy).

### Not the app, but good to know

- **YouTube.** When you play a YouTube video on a TV, the app tells the TV to open it. The TV then talks to YouTube, as
  when you use the TV's own YouTube app. The app itself doesn't contact YouTube.
- **Your devices' own internet use.** Some commands make a device contact its maker, for example "check for updates"
  on a smart plug, or opening a web address on a TV. That traffic is between the device and its maker.
- **Accounts with device makers.** We have no accounts. A few devices, such as TP-Link Tapo plugs and Roborock or
  Dreame robot vacuums, need a login or a token that comes from the maker's own cloud account, which you set up in the
  maker's app. This app doesn't create such accounts and doesn't contact the maker's cloud; it uses the login or token
  only to talk to the device on your home network.
- **Pictures on the Cast screen.** The app shows cover art only when it comes from a device on your home network. It
  never fetches images from the internet.
- **Opening a device's web page** hands the address to your browser, which loads the page from the device on your
  network.
- **Spoken announcements** are made by the text-to-speech engine chosen in your phone's settings. The app doesn't ask
  for a cloud voice, but the engine's own settings apply.

## What your devices see

When the app finds or controls a device, that device sees the phone's local IP address and, depending on Android's
"randomised MAC" setting, its Wi-Fi MAC address. When you pair a Bluetooth device, it sees your phone's Bluetooth name,
as with any pairing. The app adds nothing about you:

| Where | What the device receives | Why |
|---|---|---|
| HTTP `User-Agent` (UPnP descriptions, Samsung, Kodi, Sonos, Bose, Sony, Panasonic and others) | `Remote` | Android's default would name the phone model and build. |
| SSDP search | the standard search only, no `USER-AGENT` header | The header is optional in UPnP. |
| mDNS | queries only; the app announces no service | |
| Samsung TV remote name | `Remote` | Shown on the TV's Allow prompt. |
| Android TV pairing name | `remote` / `Phone remote` | Shown on the TV once. |
| LG TV pairing | no name; the TV shows its standard prompt | |
| Android TV client certificate | `CN=remote` | Made in the Android Keystore; no personal data. |
| ADB public key comment | `remote@phone` | The box lists it under "Allowed computers". |
| Network printer jobs | user name `Remote` | Printers log who printed. |
| Bluetooth LE scans | the phone's rotating random address | Android changes it regularly. The app doesn't change your Bluetooth name; it only puts back a name an earlier version masked (see "What stays on your phone"). |

**Your device logins on your home network.** A camera login is sent only to that camera's saved address, and only
after the camera asks for it; the app prefers Digest authentication, which doesn't send the password itself. Many cameras, printers and older devices only accept plain HTTP or RTSP,
so the login you saved for them travels unencrypted on your own Wi-Fi, as it does with the maker's own app. If you
tap "Open live stream in a video player", the stream address, including that camera's login, is handed to the player
app you pick; that app then connects to the camera itself.

The scanner only listens to what devices announce and reads their public descriptions. It doesn't connect to a device
or open a remote session until you choose it. Bluetooth pairing happens only when you choose a device and tap Pair.

**Quiet discovery (developer option).** Wi-Fi discovery then only listens for announcements devices send on their own
(SSDP NOTIFY). It sends no searches, mDNS queries or broadcasts, fetches no descriptions and doesn't probe addresses
you added. Fewer devices appear, and slowly, because devices re-announce only every 15 to 30 minutes or so.

## Permissions

- **Nearby devices (Bluetooth)**, Android 12 and newer: to find and connect to Bluetooth devices. The app declares to
  Android that it doesn't use Bluetooth to find your location.
- **Location**, Android 11 and older only: Android requires it for Bluetooth scanning. The app doesn't read your
  location.
- **Network access and Wi-Fi multicast**: to find and control devices on your Wi-Fi.
- **Google Play billing**: for the Pro purchase.

## Children

The app is not meant for children: it controls mains power, locks and moving furniture.

## Your choices

We hold no data about you, so there's nothing for us to hand over, correct or delete. Everything is on your phone and
in your control:

- "Forget device" removes a saved device with its login and, for Wi-Fi devices, its certificate fingerprint.
- Android's Settings › Apps › Universal Remote › Storage › Clear storage removes everything the app saved.
- Uninstalling removes everything, including the Keystore keys.
- For data Google holds about your purchase or the billing reports, contact Google or use your Google account's
  privacy settings.

## Law and your rights

Gdato publishes the app from Switzerland and follows the Swiss Federal Act on Data Protection (FADP) and, for users in
the EU and EEA, the General Data Protection Regulation (GDPR). The app keeps your data on your phone and sends us
nothing, so we hold no personal data about you to show, correct or delete. You remove everything by forgetting a
device or uninstalling the app (see "Your choices"). For what Google Play processes, Google is responsible; see
Google's privacy policy. You can contact us with any question, and you can complain to the Swiss Federal Data
Protection and Information Commissioner (FDPIC) or to the data protection authority where you live.

## Changes

If the app changes how it handles data, we'll update this policy and its effective date first. A change to the three
promises will be shown in the app before it applies.

## Contact

guillermodato@gmail.com
