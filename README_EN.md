# WebADB Console

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![WebUSB](https://img.shields.io/badge/WebUSB-Enabled-0284c7?logo=usb&logoColor=white)]()
[![Zero Dependency](https://img.shields.io/badge/Zero-Dependency-10b981)]()
[![Pure Frontend](https://img.shields.io/badge/Pure-Frontend-6366f1)]()
[![i18n](https://img.shields.io/badge/i18n-ZH%2FEN-38bdf8)]()
[![GitHub last commit](https://img.shields.io/github/last-commit/aoooa101/aoooa-webadb)](https://github.com/aoooa101/aoooa-webadb)
[![GitHub stars](https://img.shields.io/github/stars/aoooa101/aoooa-webadb)](https://github.com/aoooa101/aoooa-webadb)

[简体中文](README.md) | **English**

**Live Demo**: [webadb.586251.xyz](https://webadb.586251.xyz) (Recommended)  
**Alternative Entry**: [https://aoooa101.github.io/aoooa-webadb/](https://aoooa101.github.io/aoooa-webadb/)

A driverless browser-based ADB tool powered by WebUSB. Connect your phone via USB cable to activate Shizuku, Dhizuku, or run ADB commands directly in your browser.

## Features

- **Framework Activation**: Supports auto-detecting and starting Shizuku, as well as one-click autofill for Dhizuku / Hail / StopApp / IceBox / Brevent / Thanox activation commands.
- **Wireless Debugging**: One-click enable/disable wireless ADB on port 5555 via ADB protocol commands (non-root available).
- **Device Information**: Automatically reads device model, Android version, battery level, and SELinux status upon connection.
- **Custom Commands**: Supports arbitrary shell commands (automatically strips redundant `adb shell` prefixes from pasted text, press Enter to execute).
- **Pure Frontend Execution**: No backend, no data collection, direct connection via the browser's native WebUSB API, dependencies are bundled locally with zero external requests.
- **Multilingual**: Automatically switches to Chinese or English based on browser language.

## Deployment

This project requires no build steps and no Node.js installation. Simply place `index.html` together with the `vendor/` directory on any static web server (such as GitHub Pages, Cloudflare Pages, or Nginx) (the page has built-in Chinese/English switching, no additional files required).

> **Note**: WebUSB API requires the page to be served over HTTPS or on `http://localhost`.

## Want More Features?

For more features and capabilities, please use the APP version:

- **APP Repository**: [aoooa101/aoooa-adb-android](https://github.com/aoooa101/aoooa-adb-android)

## Acknowledgments

This project is built upon the following open-source project:

- [ya-webadb](https://github.com/yume-chan/ya-webadb) (@yume-chan/adb series) — In-browser ADB protocol implementation and WebUSB connection layer (MIT License). Dependencies are bundled locally as `vendor/adb-bundle.js`, requiring no external requests during runtime.

## Disclaimer

This tool is intended for technical research and daily personal usage only. ADB grants system-level privileges; please verify high-risk commands before execution. Users assume full responsibility for any device anomalies resulting from misuse.

## License

This project is open-sourced under the [GPL-3.0](./LICENSE) license. Any derivative work based on this project must remain open-sourced under GPL-3.0 when distributed.

Author: aoooa
