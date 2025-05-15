# USER GUIDE

## 1. App Overview and Main Navigation

The Benchminer app features five primary tabs located at the bottom of the screen:

- **Info**: View device specifications and supported algorithms
- **Bench**: Select and run benchmark tests
- **Miner**: Configure and launch mining sessions
- **Cluster**: Distributed mining using multiple devices over a local network
- **About**: View version and license information

![navigation](images/navigation_bar.png)

---

## 2. Info - Device Specifications

This page displays technical details of your device including model, OS version, CPU, RAM, and GPU.  
It also shows a compatibility table listing which algorithms are supported on your device by CPU or GPU.

![info](images/info_device_support.png)

---

## 3. Bench - Running Benchmarks

1. Select one or more benchmark configurations, combining an algorithm with a compute backend (CPU/GPU).
   - Example: verushash (CPU - Multi), sha256d (CPU - Single)
   - Use **Select All** to run all benchmarks.
2. Tap the **RUN BENCHMARK** button to begin testing.
3. Each selected test takes approximately **1 minute** to complete.
4. After all tests finish, the app displays performance scores and stores average hashrates for future reference.

![benchmark](images/benchmark_selection.png)

---

## 4. Miner - Starting a Mining Session

1. **Select or create a Stratum Preset**  
   Presets store mining settings. Tap **CREATE** to define a new one:
   - **Preset Title**: A label to distinguish this preset
   - **Algorithm Name**: Choose the hash algorithm (e.g., verushash, ghostrider, sha256d)
   - **Pool URL**: The address of the Stratum pool  
     Supports TCP or SSL, such as:  
     `stratum+tcp://your.pool.address:port`  
     `stratum+ssl://your.pool.address:port`  
     `your.pool.address:port`
   - **Wallet Address**: Your wallet address to receive rewards
   - **Worker Name / Password** (optional): Identifies your device to the pool
2. **Choose compute backend**  
   Select CPU or GPU as the mining backend (depending on device support)
3. Tap **START MINING** to begin
4. The app will display real-time mining metrics:
   - Algorithm, pool URL, current hashrate, submitted shares, error count, etc.

![miner_empty](images/miner_empty.png)
![preset_edit](images/preset_edit.png)
![miner_ready](images/miner_ready.png)
![miner_running](images/miner_running.png)

---

## 5. Cluster - Distributed Mining Mode

Cluster mode allows you to distribute mining jobs across multiple devices in the same local network.

### Cluster Server Mode

- Acts as a central job coordinator
- Connects to a Stratum pool and distributes mining jobs to other devices
- Does not mine itself
- Required settings:
  - **Select a Stratum preset**
  - **Listening Port**: Port for incoming node connections
  - **Local IP Address**: Auto-detected for display

![cluster_server](images/cluster_server.png)

### Cluster Node Mode

- Connects to a Cluster Server and performs mining work assigned by the server
- Required settings:
  - **Server IP**: IP address of the Cluster Server
  - **Server Port**: Must match the server’s listening port
  - **Nickname**: Friendly name to identify the device in the cluster

![cluster_node](images/cluster_node.png)

---

## 6. Preset Management Tips

- The same preset list is shared between Miner and Cluster modes
- Up to **5 presets** can be stored
- Use the **+** button to add a new preset
- Presets can be edited or deleted anytime and persist after app restarts

![preset_slots](images/preset_slots.png)

---

## 7. Troubleshooting Guide

- **Mining won't start**  
  → Verify the Pool URL, Wallet Address, and compute backend settings

- **GPU backend doesn't work**  
  → Check whether the selected algorithm supports GPU on your device

- **Benchmark shows zero or very low results**  
  → Try different backends or verify that your device supports the algorithm

- **Cluster Node cannot connect**  
  → Double-check server IP, port, and local network connection
