# Cafari

A casting browser for iPhone: send web video to a Chromecast, an AirPlay
receiver, or the car's CarPlay screen.

## Install

Download the `.ipa` from the [latest release](../../releases/latest) and
sideload it with AltStore, SideStore or Sideloadly.

**Builds expire 90 days after they are made.** The expiry date is in the file
name, and the app warns for the last two weeks before it stops working.

**About the car screen:** when you re-sign the app with your own Apple ID,
which every sideloading tool does, it loses the CarPlay entitlements that
belong to VMLite. Casting to Chromecast and AirPlay receivers still works;
video on the car's own screen needs a build signed by us (TestFlight).

## What it does

- **YouTube to the car** at the quality the page plays, with the queue playing
  on by itself. A 360p mode is available in Settings for a simpler path.
- **Cast tab** — the page's picture and sound to a Chromecast, an AirPlay
  receiver or the car screen.
- **Cast Screen** — the whole phone, other apps included, through the system
  recorder.
- **Car screen options** in Settings: how video fills the screen, and which
  side the CarPlay sidebar is on.

Video on the car screen appears only while the car is parked.

## Reporting a problem

Settings, then Advanced, then **Send debug log**. It carries the last few runs
and is what makes a bug fixable. It records the addresses of pages you visited,
so look it over before sharing.
