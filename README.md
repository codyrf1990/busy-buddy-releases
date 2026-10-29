# Busy Buddy

Sets your Microsoft Teams status to **Busy · In a call** while you're on a browser call (HubSpot calling in Chrome, Edge, Firefox, Brave, Comet, Helium and similar), and puts it back when you hang up. It lives in the Windows tray and updates itself.

## Install

1. Download **[BusyBuddy-Setup.exe](https://github.com/codyrf1990/busy-buddy-releases/releases/latest/download/BusyBuddy-Setup.exe)**.
2. Run it. It installs just for you (no admin rights needed).
3. Windows SmartScreen may say "Windows protected your PC" because the installer isn't code-signed. Click **More info**, then **Run anyway**.
4. Click the tray icon (green microphone, near the clock; it may sit under the **^** arrow) and press **Sign in**. Sign in with your work Microsoft account and accept the one permission it asks for.

That's it. Start a call in your browser and Teams shows Busy about a second later; hang up and it clears about a second after.

## What it can see and do

- It reads which program is using your microphone (a Windows list; it never records or hears audio) and only reacts to web browsers.
- With your sign-in it can read and change **your own Teams presence**, nothing else: the single Microsoft Graph permission is `Presence.ReadWrite`. It can't see your mail, calendar, chats or files, or anyone else's status.
- Optional, off by default: a status message and Do Not Disturb while you're on a call.
- Your sign-in is stored on your PC, encrypted with Windows' own key protection. Uninstalling deletes it. Nothing is sent anywhere except to Microsoft and to GitHub (to check for updates).
- If your company blocks apps from asking for that permission, sign-in will say so and nothing is changed.

## Updates

The app checks this page about once an hour, verifies the download's checksum, and installs a new version quietly when you're not on a call. The footer of the panel shows the version.

## Uninstall

Windows Settings > Apps > Busy Buddy.

---
Releases only; the source is private.
