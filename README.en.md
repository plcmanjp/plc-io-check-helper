# PLC Field Notebook

[한국어](README.md) | **English**

**Check MELSEC PLC I/O and record inspection results from your Android phone.**

PLC Field Notebook (formerly PLC IO Check) helps you inspect I/O, monitor device values and perform engineering calculations in the field. It reads values directly through MC Protocol/SLMP over a network that can reach your PLC.

**[Install from Google Play](https://play.google.com/store/apps/details?id=com.plciocheck.iocheck&hl=en)** | [Product website](https://plcmanjp.github.io/plc-io-check-helper/) | [Report a problem or suggest a feature](https://github.com/plcmanjp/plc-io-check-helper/issues/new/choose)

Requires Android 8.0 or later. Check Google Play for the latest release and device compatibility. This repository provides product information and help links; it does not distribute the app source code or installation files.

## What you can do

| Your task | How the app helps |
| --- | --- |
| Inspect sensors and output signals | Check X/Y I/O and record OK/NG verdicts and inspection results. |
| Read several device values together | Monitor bit states and word values, or use the batch monitor to view addresses in a table. |
| Organize addresses and comments by machine | Save projects and groups, then find items with search and status filters. |
| Record changes in values | Use the simple logger to record events by condition or interval. |
| Run calculations and inspect codes on site | Use built-in tools for number bases, analog scaling, checksums, CRC and more. |

## Preview

| Device monitor | IO check | Batch monitor |
| :---: | :---: | :---: |
| <img src="assets/app-monitor.png" width="220" alt="Device monitor showing device addresses and values"> | <img src="assets/app-iocheck.png" width="220" alt="IO check screen for input and output inspection"> | <img src="assets/app-batch.png" width="220" alt="Batch monitor showing multiple addresses in a table"> |

Screen layouts may vary by app version and settings. Preview images may use a different display language.

## Get started

1. **Install the app.** Find `PLC Field Notebook: MELSEC I/O` on Google Play.
2. **Prepare the connection.** Your phone needs network access to the PLC's IP address and port. Check the PLC's Ethernet and MC Protocol/SLMP settings as well.
3. **Set up a project and connection.** Match the PLC model, IP address, port and communication format to the actual equipment. The connection screen includes a guide to GX Works communication settings.
4. **Register devices.** Enter addresses manually or add them in batches. To reuse existing comments, importing a comment CSV exported from GX Works is recommended.
5. **Read values and inspect I/O.** Start monitoring, confirm that values are being read and record verdicts in IO check. Apply physical signals separately according to your site's safety procedures.

If the connection fails, first check that the PLC's IP address, port, TCP/UDP, frame and data format match the app settings.

## Features

- **IO check:** Inspect in manual, automatic or guided sequential mode, then share results as CSV files and summary reports.
- **Device monitoring:** Read bit states such as X/Y/M/L/B and word values such as D/W/ZR. Display words as decimal, hexadecimal, signed, 32-bit, floating-point or string values.
- **Projects and groups:** Organize machines with projects, hierarchical groups, search and status filters. Share projects as `.plc` files.
- **GX Works import:** Import devices and comments from comment/ladder CSV, GX Works2 `.gxw` and supported GX Works3 FX5U `.gx3` files. Not all GX3 models or data formats are supported; unsupported projects are rejected without registration.
- **Simple logger and HMI:** Record events by condition or interval, display values, animate movement and show elements based on bit states.
- **11 engineering tools:** Programmer calculator, electronic gear ratio, circumference, trigonometry, analog scaling, communication codes, serial transmission time, UVW stage, Modbus RTU frame generator, ASCII table and ASCII input. Some are also available in the [web engineering tools](https://plcmanjp.github.io/engineer-tool/).
- **Languages and themes:** Korean, English, Japanese, Simplified Chinese, Traditional Chinese and Vietnamese, with light and dark themes.

## PLC connections and protocols

| Item | Details |
| --- | --- |
| MELSEC Q | Verified configurations include the QJ71E71-100 module and QnUDV CPU built-in Ethernet. |
| MELSEC iQ-R | Verified configurations include the RJ71EN71 module and CPU built-in Ethernet. |
| Protocols | MC Protocol/SLMP, TCP/UDP, 3E/4E frames and Binary/ASCII. |

Connectivity and readable device ranges depend on the CPU, communication module and PLC configuration. File import support and live communication support are separate capabilities.

## Free use and ads

- Basic IO check, monitoring, opening/viewing/recording in the simple logger and calculator tools are free.
- Device registration is unlimited. Free monitoring covers the first 50 active devices in the list.
- A bottom banner ad is displayed. Completing an optional rewarded ad grants one token.
- One token is used for a successful LOG/IO CSV save, GX Works device registration/comment merge, or 12 hours without the bottom banner. Failed, cancelled or zero-change operations do not consume a token.
- There are no in-app purchases or cash rewards.

## Help and feedback

The following articles are in Korean:

- [App overview and features](https://plcman.tistory.com/236)
- [Q-series connection and IO monitoring guide](https://plcman.tistory.com/237)
- [GX Works CSV device registration guide](https://plcman.tistory.com/238)
- [Web engineering tools guide](https://plcman.tistory.com/255)

[Report a problem or suggest a feature](https://github.com/plcmanjp/plc-io-check-helper/issues/new/choose) | [Privacy policy (Korean and English)](https://plcmanjp.github.io/plc-io-check-helper/privacy/)

For a bug report, include the app version, Android version, PLC model and steps to reproduce. Issues are public: please do not post customer information, real equipment IP addresses or private project files.

## Before using the app

The app is a **read-only monitoring tool**. It does not write PLC values or force outputs on. Automatic IO check assists inspection; it does not operate the equipment automatically.

This is an independent third-party app, with no affiliation, endorsement or approval from Mitsubishi Electric Corporation. MELSEC, GX Works and related names are trademarks of their respective owners and are used only to describe compatibility.

GX Works project import is an unofficial compatibility feature that extracts devices and comments from files you own. Results may omit data or interpret it differently, so verify them before use in the field. For accurate data, exporting a comment CSV from GX Works and importing that file is recommended. Password-protected or protected files are not opened or bypassed.
