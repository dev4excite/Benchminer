# Benchminer Project Overview

**Benchminer** is a mobile tool for Android devices that allows users to measure the performance of various hash algorithms (Benchmark) and to perform actual mining by connecting to a Stratum-compatible mining pool.  
This repository serves as the **official APK distribution channel** for Benchminer, providing the **full-featured version** that includes both Benchmark and Mining functionalities.

> Note: The version available on Google Play includes only the Benchmark feature, as Mining is restricted by Google Play policies.

---

## Distributed Files

- `benchminer-vX.X.X-full.apk`: Official release APK with both Benchmark and Mining features
- For version history and details, see the Releases tab on GitHub

---

## Key Features

- Measure hashrate performance for multiple hash algorithms
- Perform mining using CPU or GPU backends
- Real-time session reporting and performance summary

---

## Supported Algorithms and Backends (as of v2.x.x)

| Algorithm   | CPU | OpenCL | Vulkan | Metal | Cuda |
|-------------|:---:|:------:|:------:|:-----:|:----:|
| Sha256d     | O   |        |        |       |      |
| Verushash   | O   |   O    |        |       |      |
| Ghostrider  | O   |        |        |       |      |

> Availability of GPU backends (OpenCL, Vulkan, Metal, Cuda) depends on device and platform support.

---

## Installation Instructions

1. Download the `.apk` file from the Releases section above
2. On your Android device, allow **"Install unknown apps"**
3. Run and install the `.apk` file

---

## User Guide

For detailed instructions on how to configure and run Benchminer, please refer to the user guide below.  
[USER_GUIDE.md](USER_GUIDE.md)

---

## Google Play Version

Due to policy limitations, the Google Play version of Benchminer includes only the Benchmark feature and excludes mining.

Google Play link: [Benchminer (Benchmark only)](https://play.google.com/store/apps/details?id=com.dev4excite.benchminer.bench)

---

## Developer Fee (Dev Fee)

When using Benchminer for mining, 3 percent of the total mining time is allocated to the developer.  
For example, if a user mines for 100 minutes, approximately 3 minutes will be used to mine on behalf of the developer.  
This fee supports ongoing development and maintenance of the project.

---

## License

This APK is provided by dev4excite under a custom license.  
Usage is allowed for both personal and commercial purposes, but redistribution and modification are prohibited.  
See [LICENSE](LICENSE) for full terms.
