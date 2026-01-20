# Benchminer

Cryptocurrency mining and benchmarking app for Android devices.

[benchminer.com](https://benchminer.com)

This repository provides the **Full Version** with both benchmark and mining features.

## Download

Download the latest APK from the [Releases](https://github.com/dev4excite/Benchminer/releases) tab.

## Features

- **Benchmarking**: Measure hashrate for each algorithm on your device
- **Profit Estimation**: View estimated monthly earnings based on measured hashrate
- **Mining**: Connect to mining pools and mine cryptocurrency
- **Cluster Mode**: Connect multiple devices for distributed mining

## Supported Algorithms

| Algorithm | CPU | OpenCL | Vulkan | Metal | Cuda |
|-----------|-----|--------|--------|-------|------|
| SHA256d | O | - | - | - | - |
| Verushash | O | O | - | - | - |
| Ghostrider | O | - | - | - | - |
| RandomX | O | - | - | - | - |

> **Note:** RandomX is supported from v3.x.x.

GPU backend support (OpenCL, Vulkan, Metal, Cuda) varies by device. Check the **Info** tab in the app.

## System Requirements

- Android 6.0 (Marshmallow) or higher
- Minimum 2GB RAM
- 100MB+ storage space

## Permissions

- Internet access (mining pool connection)
- Network state (connection monitoring)

## Installation

1. Download the latest APK from [Releases](https://github.com/dev4excite/Benchminer/releases)
2. Enable "Unknown sources" installation (Settings > Security)
3. Install the APK

## Quick Start

1. **Run Benchmark** → Measure performance for each algorithm in the Bench tab
2. **Choose a Coin** → Decide which coin to mine based on profitability results
3. **Prepare Wallet/Pool** → Set up a wallet and find a mining pool for your chosen coin
4. **Start Mining** → Configure settings in the Miner tab and start

For detailed instructions, see [USER_GUIDE.md](USER_GUIDE.md).

## Google Play Version

The [Google Play version](https://play.google.com/store/apps/details?id=com.dev4excite.benchminer.bench) includes **benchmark features only** due to policy restrictions. Download the Full Version APK from this repository to use mining features.

## Developer Fee

A **3%** developer fee is applied to mining time. This supports ongoing development and maintenance.

## FAQ

**Q: Is this app safe?**
A: The app only performs mining operations and does not collect personal information or harm your device. Wallet addresses are used solely for pool connections and stored locally on your device.

**Q: Can I make money mining on a mobile device?**
A: Mobile devices have lower hashrates compared to dedicated mining hardware. Check the estimated profit from benchmark results and consider electricity costs before deciding.

**Q: What's the difference from the Google Play version?**
A: The Google Play version only provides benchmark features due to policy restrictions. The Full Version from this repository includes mining and cluster features.

## License

Copyright (c) dev4excite. All rights reserved.

This software may be used for personal and commercial purposes. Redistribution and modification are not permitted. See the [LICENSE](LICENSE) file for details.
