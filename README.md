# Cafari

A casting browser: send web video to a Chromecast, an AirPlay receiver, or the
car's screen.

## Cafari for iOS

### Install

Download the `.ipa` from the [latest release](../../releases/latest) and
sideload it with AltStore, SideStore or Sideloadly.

**iOS versions:** works on iOS 26.4 and later, and on iOS 27.0. Not yet on
the iOS 27.2 beta.

**Builds expire 90 days after they are made.** The expiry date is in the file
name, and the app warns for the last two weeks before it stops working.

**About the car screen:** casting to Chromecast and AirPlay receivers works
with any signing. Video on the car's own CarPlay screen depends on how the
build is signed, and re-signing with your own Apple ID may lose it. Some
people report it working, so try it; if the car screen stays empty, that is
why, and a build signed by us (TestFlight) will have it.

#### Getting the car screen with your own signing

CarPlay entitlements are granted by Apple, per developer account, and a
sideloaded build carries whatever the account signing it has. If you want the
car screen on a build you sign yourself:

1. You need a paid Apple Developer account ($99/year). A free Apple ID cannot
   hold CarPlay entitlements.
2. Ask Apple for them: <https://developer.apple.com/contact/carplay/>. Request
   the **audio** and **video** CarPlay app entitlements, and say what the app
   does — a browser that plays video on the car screen while parked.
3. Apple answers by email. Approval is not automatic, and they grant these for
   app categories they have decided to support.
4. If granted, the entitlements appear against your account. Create a
   provisioning profile that includes them and re-sign the `.ipa` with it.

Background on the entitlements is at <https://developer.apple.com/carplay/>.

### What it does

- **YouTube to the car** at the quality the page plays, with the queue playing
  on by itself. A 360p mode is available in Settings for a simpler path.
- **Cast tab** — the page's picture and sound to a Chromecast, an AirPlay
  receiver or the car screen.
- **Cast Screen** — the whole phone, other apps included, through the system
  recorder.
- **Car screen options** in Settings: how video fills the screen, and which
  side the CarPlay sidebar is on.

Video on the car screen appears only while the car is parked (the check is
switched off at the moment, so video plays regardless).

### Reporting a problem

Settings, then Advanced, then **Send debug log**. It carries the last few runs
and is what makes a bug fixable. It records the addresses of pages you visited,
so look it over before sharing.

## Cafari for Android

An Android build is in the works, with the same casting: YouTube and web video
to a Chromecast, an AirPlay receiver, or the car screen over Android Auto and
wireless CarPlay boxes.

The `.apk` will be published here as a release when it is ready. Watch this
repository to be told about it.
