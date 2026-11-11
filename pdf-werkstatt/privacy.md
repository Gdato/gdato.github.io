---
title: "PDF Werkstatt: privacy policy"
permalink: /pdf-werkstatt/privacy
---

# PDF Werkstatt: privacy policy

Effective date: 11 November 2026  
Publisher: Gdato, Switzerland  
Contact: guillermodato@gmail.com

This policy is for the Android app "PDF Werkstatt" (package `com.gdato.pdfwerkstatt`) in both editions: the one on
Google Play and the one distributed outside it. It goes with the [terms of use](terms.md).

## The short version

- **Your files never leave the phone.** The app has no server. Creating, converting and editing PDFs all happen on
  the phone itself. A file goes somewhere else only when you save or share it yourself.
- **No tracking.** No account with us, no analytics, no advertising ID, no crash reporting. We receive nothing about
  you, your phone or your documents.
- **No ads.** There is no advertising code in the app.
- **No hidden processes.** We wrote no background service, scheduled task or start-with-the-phone code. The app works
  only while it is open, with one exception in the Google Play edition that comes from Google, not from us: Google's
  billing library may send its own technical report to Google a little later.

There are three things you should know about, and they apply only to the Google Play edition: Google Play for tips,
with the reports of the **Google Play Billing library**, which apps that sell through Google Play build in; Google's
document scanner; and the website you ask the app to turn into a PDF. They are described under "What leaves your
phone".

## What stays on your phone

Everything the app knows is kept in its private storage on your phone, which other apps can't read:

| What | Why | Where |
|---|---|---|
| Settings (appearance including the colour palette, language, text size, paper size, screen and vibration options), and that you have seen the welcome screens | To remember your choices | App storage |
| The count of created PDFs, and which tip prompts were shown and when | So the app can ask, once in a while and not too often, whether you would like to leave a tip. Only the number and the dates are kept, nothing about the files | App storage |
| Whether you are a supporter (Google Play edition) | So the supporter colour palettes work offline | App storage |
| Temporary files: copies of the files you picked, pictures from the scanner, working files and the finished PDFs shown under "Recent" | To do the job you asked for, and to let you save, share or open the result | App cache |

**How long temporary files are kept.** Copies of your input files and working files are deleted as soon as a job has
finished, failed or been cancelled. The one exception: for a PDF you protected with a password, the app keeps an
unprotected copy so it can show you the preview; that copy is deleted together with the result. A finished PDF is
deleted when you remove it from "Recent", when more than 10 results have pushed it out of that list, and when you
close the app. No temporary file is kept longer than 24 hours while the app is in use. Anything left over after a
crash is deleted the next time the app starts. Android may also clear the cache at any time. The app has no
background work, so it cannot delete anything while it is not running: if Android stops the app in the background,
the leftovers stay until you open the app again.

The app keeps no history database and no list of file names. When a result is gone from "Recent", the app knows
nothing about it any more.

**Files you save or share.** A PDF you save goes only where you choose in Android's own save dialog. If that is a
cloud folder, that service's privacy terms apply. When you share a PDF or open it with another app, only that app
gets temporary permission to read that one file.

The app doesn't use your location, contacts, photos or files, except the ones you pick yourself or share to the app
from another app.

## Android backup

If you have turned on backup to your Google account in Android's settings, or you move to a new phone, Android may
copy the app's settings, and with them the count of created PDFs and which tip prompts were shown and when, which
are kept in the same place. Nothing else is included: no documents, no temporary files and not the supporter flag.
This is Android's feature under Google's terms; you can turn it off in Android's settings.

## What leaves your phone (Google Play edition)

Your documents don't. These are the only three ways the Google Play edition talks to anything outside the phone. The
first has two parts: what the app asks Google Play, and what Google's billing library reports by itself.

### 1. Google Play, for tips

Tips and the one-time supporter thank-you are purchases through Google Play. Google processes the payment and holds
your payment details; we never see them. We only learn, through the billing library, that a purchase happened, so the
app can thank you and, for the supporter thank-you, remember it on your phone.

The app asks the Google Play app on your phone about purchases each time the app comes to the foreground (to finish a
tip that was interrupted and to confirm the supporter thank-you), when you open the support sheet and when you leave a
tip.

Purchases can be restored on another phone signed in to the same Google account ("Restore purchases" in the support
sheet).

**Google Play Billing library reports.** The Play Billing library, written and supplied by Google, is part of the
Google Play edition. It talks to Google Play on the phone, and it sends technical reports about its own work (for
example which billing step ran and its result, and the library version) to Google's logging service at
`firebaselogging.googleapis.com` and `firebaselogging-pa.googleapis.com`. The library decides what goes in these
reports, not us. It uses Android's job scheduler, so a report may be sent a little later, also while the app isn't
open. Because the app asks Google Play about purchases each time it comes to the foreground, this applies to everyone
who uses the Google Play edition, also if you never leave a tip. We don't receive these reports and can't see them.

Both are covered by [Google's privacy policy](https://policies.google.com/privacy).

### 2. The Google document scanner

In the Google Play edition, the scanner is Google's document scanner (ML Kit), a part of Google Play services.

- The pictures you take are processed on the phone. They are not sent to Google.
- Google Play services downloads the scanner once.
- Google receives metrics about the performance and use of the scanner: device and app information, a
  per-installation identifier, latency, configuration and error codes. They contain no pictures.

We don't receive these metrics and can't see them. They are covered by
[Google's privacy policy](https://policies.google.com/privacy).

### 3. Web pages

When you ask the app to turn a web page into a PDF, the app loads that page with Android's built-in web component
(Android System WebView) and prints it to a PDF on the phone.

- The website you name is contacted directly, as a browser would do it. It sees your IP address and a browser user
  agent. A page can also load parts of itself, such as pictures or fonts, from other servers, which then see the same.
- A web address that starts with `http://` is tried over `https://` instead. The app does not use plain, unencrypted
  connections.
- Google Safe Browsing, which is part of Android's web component, checks the addresses of the pages it loads against
  Google's list of dangerous sites. Depending on the address, this check can involve Google's servers; see
  [Google's privacy policy](https://policies.google.com/privacy).
- Cookies and other data the page stores are deleted when the conversion ends. Pages behind a login can't be
  converted.

Nothing is sent to us, and the app itself contacts no other website.

## The edition outside Google Play

The edition distributed outside Google Play contains no Google code and has no internet permission, so none of the
three points above applies to it: it has no Google Play Billing and no Google scanner, and it cannot load web pages.
It scans with its own camera screen, on the phone. Its support screen opens the [support page](support.md) in your
browser; what happens on a payment page you open from there is governed by that service's own policy.

## Permissions

- **Camera**: only in the edition outside Google Play, and only on the scanner screen. Android asks you when you
  open the scanner for the first time. The Google Play edition has no camera permission: there the camera is used by
  Google's scanner in Google Play services.
- **Network access and Google Play billing**: only in the Google Play edition, for the three things described above.
- **No storage permission** in either edition. The app sees only the files you pick with Android's own picker or
  share to it from another app, and writes only where you save with Android's own dialog.

## Children

The app is not directed at children under 13. We collect no data from anyone; what Google's components receive is
described above.

## Your choices

We hold no data about you, so there's nothing for us to hand over, correct or delete. Everything is on your phone and
in your control:

- Removing a result from "Recent" deletes that file. Closing the app deletes all results.
- Android's Settings › Apps › PDF Werkstatt › Storage › Clear storage removes everything the app saved.
- Uninstalling removes everything.
- For data Google holds about a purchase, the billing reports or the scanner metrics, contact Google or use your
  Google account's privacy settings.

## Law and your rights

Gdato publishes the app from Switzerland and follows the Swiss Federal Act on Data Protection (FADP) and, for users in
the EU and EEA, the General Data Protection Regulation (GDPR). The app keeps your data on your phone and sends us
nothing, so we hold no personal data about you to show, correct or delete. You remove everything by clearing the
app's storage or uninstalling the app (see "Your choices"). For what Google processes through Google Play, Google
Play services and Safe Browsing, Google is responsible; see Google's privacy policy. For what a website learns when
you convert one of its pages, that website is responsible. You can contact us with any question, and you can complain
to the Swiss Federal Data Protection and Information Commissioner (FDPIC) or to the data protection authority where
you live.

## Changes

If the app changes how it handles data, we'll update this policy and its effective date first. A change to the
promises will be shown in the app before it applies. The app's About screen links here.

## Contact

guillermodato@gmail.com
