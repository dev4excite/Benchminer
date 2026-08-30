# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [v4.2.1] - 2026-08-30

Cumulative release since v3.1.1. Mining engine updated from 3.1.1 to 4.2.1.

### Added
- AstroBWT v3 algorithm (CPU) with Dero support
- Dero pool connectivity: native Dero protocol, Stratum, and WebSocket/WSS (`ws://`, `wss://`) connections
- VerusHash support on all CPU architectures, including those without hardware AES
- Automatic mining pause and resume based on battery level, configurable from the overflow menu
- CPU worker count setting
- RandomX execution mode (JIT / full memory) shown in benchmark and mining, and recorded with the benchmark score
- Battery settings translated into 12 languages

### Changed
- Cluster work distribution rebuilt on a new job pipeline for more reliable job delivery across nodes
- RandomX full memory mode is gated by available physical RAM, and an explicit mode the device cannot support now fails clearly instead of silently falling back
- Default worker password is `x` when left empty
- Google Play (Lite) build targets Android 16

### Fixed
- NiceHash compatibility for SHA256d and RandomX mining
- Crashes and memory leaks in RandomX dataset rebuild, socket reconnect, and share submission paths
- Large Stratum messages split across packets being dropped
- RandomX rejecting jobs with large blobs
- AstroBWT nonce not advancing past a found share
- Benchmark result mislabeled when an entry failed
- RAM displayed incorrectly when reported in bytes
- Cluster node worker name and hardcoded algorithm
- Battery card missing from landscape layout

## [v3.1.1] - 2026-03-03
### Changed
- New app icon and splash screen

### Fixed
- Benchmark crash fixes and stability improvements
- Network compatibility fix for Android 7.0

## [v3.0.5] - 2026-01-13
### Fixed
- Input text trim and sanitization

## [v3.0.4] - 2026-01-03
### Added
- RandomX algorithm support (CPU)
- Monthly profit estimation based on benchmark results

### Changed
- UI/UX improvements
- Updated user guide with improved structure
- Simplified wallet and pool setup instructions

### Fixed
- Bug fixes

## [v2.1.7] - 2025-06-17
### Changed
- Improved UI/UX in BenchFragment

## [v2.1.3] - 2025-05-15
### Added
- Initial public release of full-featured APK (Benchmark + Mining)
- CPU algorithm: Sha256d, Verushash, Ghostrider
- GPU support (OpenCL only) for Verushash
- Stratum Preset management UI
- Real-time mining dashboard (hashrate, shares, errors)
- Cluster Server and Node modes over LAN
- 3% Dev Fee integration
