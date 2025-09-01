# Bitcoin Mining with Benchminer

## Quick Setup Guide for SHA256d Algorithm

This tutorial shows you how to set up Bitcoin mining in Benchminer using the SHA256d algorithm.

**What You Need:**
- Bitcoin wallet address 
- Bitcoin mining pool details
- Benchminer app

---

## Step 1: Get a Bitcoin Wallet

**How to Find Bitcoin Wallets:**
1. Search "bitcoin wallet" in your app store or web browser
2. Choose a reputable service (check reviews and ratings)
3. Create an account and set up your wallet
4. **Important**: Save your recovery phrase securely
5. Copy your Bitcoin receiving address (starts with "1", "3", or "bc1")

**Popular wallet types include mobile apps, web wallets, and hardware wallets.**

---

## Step 2: Find a Bitcoin Mining Pool

**How to Find Bitcoin Mining Pools:**
1. Visit **https://miningpoolstats.stream/bitcoin** to see available pools
2. Look for pools with good reputation and reasonable fees
3. Check the pool's website for setup instructions
4. Note their Stratum URL (format: `stratum+tcp://pool-address:port`)

**What to Look For:**
- Low fees (usually 1-3%)
- Variable difficulty support (good for mobile devices)
- Clear setup instructions
- Active community support

---

## Step 3: Setup in Benchminer

### Creating Your Bitcoin Preset

1. Open Benchminer → **Miner** tab
2. Tap **CREATE** to add a new preset
3. Fill in your information:

```
Preset Title: "Bitcoin Mining"
Algorithm: sha256d  
Pool URL: [Copy from your chosen pool's website]
Wallet Address: [Your Bitcoin address from Step 1]  
Worker Name: [Optional - e.g. "mobile", "phone"]
Password: [Usually "x" or blank]
```

**Tips:**
- Pool URL must include `stratum+tcp://` prefix
- Double-check your wallet address
- Worker name helps identify your device on pool dashboard
- Most pools use "x" for password (check pool's instructions)

---

## Step 4: Start Mining

1. Select your Bitcoin preset
2. Choose **CPU** as the backend (only option for SHA256d)
3. Tap **START MINING**
4. Watch the connection status and mining metrics

**What You'll See:**
- **Hashrate**: Your mining speed 
- **Shares**: Work submitted to the pool
- **Accepted/Rejected**: Success rate
- **Errors**: Connection issues (should be low)

---

## Monitoring Your Mining

**In the App:**
- Monitor hashrate and share statistics
- Check for connection errors
- Watch device temperature

**On Pool Website:**
- View detailed statistics for your worker
- Check earnings and payout information
- Configure payout settings

**Mining Tips:**
- Keep device cool during extended mining
- Use reliable WiFi connection  
- Close other apps for better performance
- Consider mining while charging

---

## Common Issues

**"Connection Failed":**
- Check pool URL format includes `stratum+tcp://`
- Verify internet connection
- Try a different pool

**"Low Performance":**
- Close background apps
- Ensure device isn't overheating
- Check if device supports higher performance

**"No Earnings":**
- Verify wallet address is correct
- Check pool's minimum payout amount
- Wait for payout schedule (usually daily/weekly)

---

## Additional Resources

**Find More Pools:**
- https://miningpoolstats.stream/bitcoin - Bitcoin pool comparison

**Learn More:**
- Visit your chosen pool's help section
- Check pool community forums for tips

---

**Note:** Keep your wallet recovery information secure and never share private keys with anyone.