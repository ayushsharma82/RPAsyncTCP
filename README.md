# RPAsyncTCP

[![GitHub release](https://img.shields.io/github/release/ayushsharma82/RPAsyncTCP.svg)](https://github.com/ayushsharma82/RPAsyncTCP/releases)
[![GitHub issues](https://img.shields.io/github/issues/ayushsharma82/RPAsyncTCP.svg)](http://github.com/ayushsharma82/RPAsyncTCP/issues)
[![arduino-library-badge](https://www.ardu-badge.com/badge/RPAsyncTCP.svg?)](https://www.ardu-badge.com/RPAsyncTCP)

---

## Disclaimer

This library is a fork of **AsyncTCP_RP2040W** and remains compatible with it. If you were previously using `AsyncTCP_RP2040W`, you will need to update your `#include` directives accordingly.

---

## Table of Contents

- [Why RPAsyncTCP?](#why-rpasynctcp)
  - [Features](#features)
  - [Why Async is better](#why-async-is-better)
  - [Supported Boards](#supported-boards)
- [Installation](#installation)
  - [Using Arduino Library Manager](#using-arduino-library-manager)
  - [Manual Installation](#manual-installation)
  - [Using VS Code & PlatformIO](#using-vs-code--platformio)
- [Examples](#examples)
- [Debugging](#debugging)
- [Troubleshooting](#troubleshooting)
- [Issues](#issues)
- [License](#license)
- [Authors & Maintainers](#authors--maintainers)

---

## Why RPAsyncTCP?

RPAsyncTCP brings the **asynchronous** networking power of ESPAsyncTCP to **RASPBERRY_PI_PICO_W with CYW43439 WiFi**, serving as the foundation for advanced libraries like `AsyncWebServer_RP2040W`.

### Features

- Handles multiple connections simultaneously
- Callbacks are triggered when requests are ready
- Faster response handling and improved efficiency
- Support for WebSockets, EventSource (Server-Sent Events), and URL Rewriting
- Static file serving with cache and indexing support
- Simple template processing

### Why Async is Better

- No blocking execution—code execution continues while data is sent
- Faster and more efficient handling of network events
- Ideal for high-performance applications requiring simultaneous client handling

### Supported Boards

- **RASPBERRY_PI_PICO_W with CYW43439 WiFi** (using [arduino-pico core](https://github.com/earlephilhower/arduino-pico))
- **Pico 2W (RP2350)**

---

## Installation

### Using Arduino Library Manager

Search for **RPAsyncTCP** in the Arduino Library Manager and install the latest version.

### Manual Installation

1. Download the latest release from [GitHub](https://github.com/ayushsharma82/RPAsyncTCP)
2. Extract and place the folder in `~/Arduino/libraries/`

### Using VS Code & PlatformIO

1. Install [VS Code](https://code.visualstudio.com/)
2. Install [PlatformIO](https://platformio.org/platformio-ide)
3. Search for **RPAsyncTCP** in the PlatformIO Library Manager and install

---

## Examples

Check out the example projects:

- [AsyncTCP_Client](https://github.com/ayushsharma82/RPAsyncTCP/tree/main/examples/ClientServer/AsyncTCP_Client)
- [AsyncTCP_Server](https://github.com/ayushsharma82/RPAsyncTCP/tree/main/examples/ClientServer/AsyncTCP_Server)

---

## Debugging

Debugging is enabled by default on Serial. You can adjust the log level by modifying `_RPAsyncTCP_LOGLEVEL_` in the library files:

```cpp
#define _RPAsyncTCP_LOGLEVEL_ 1
```

---

## Troubleshooting

If you encounter issues, ensure you are using the latest board core version. Updating may resolve compatibility problems.

---

## Issues

Report issues at: [RPAsyncTCP Issues](https://github.com/ayushsharma82/RPAsyncTCP/issues)

---

## License

This library is licensed under the [LGPL-3.0 License](LICENSE).

---

## Authors & Maintainers

- **Previous Authors:** Hristo Gochkov (2016), Khoi Hoang (2022)
- **Current Maintainer:** Ayush Sharma (2025)
