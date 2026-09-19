# Cafari

A casting browser for iPhone: send web video to a Chromecast, an AirPlay
receiver, or the car's CarPlay screen.

## Install

Download the `.ipa` from the [latest release](../../releases/latest) and
sideload it with AltStore, SideStore or Sideloadly.

**Builds expire 90 days after they are made.** The expiry date is in the file
name, and the app warns for the last two weeks before it stops working.

**About the car screen:** casting to Chromecast and AirPlay receivers works
with any signing. Video on the car's own CarPlay screen depends on how the
build is signed, and re-signing with your own Apple ID may lose it. Some
people report it working, so try it; if the car screen stays empty, that is
why, and a build signed by us (TestFlight) will have it.

## What it does

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

## Reporting a problem

Settings, then Advanced, then **Send debug log**. It carries the last few runs
and is what makes a bug fixable. It records the addresses of pages you visited,
so look it over before sharing.
