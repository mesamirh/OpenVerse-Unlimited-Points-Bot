# ⚡ OpenVerse Unlimited Points Script

This script is a fast auto-clicker designed to automate the daily reward claiming process on the [OpenVerse](https://launch.openverse.network) platform. It simulates button clicks at maximum speed, checks user balance periodically, and provides helpful debug messages in the console.

> ⚠️ **Warning**: This script runs at **maximum speed** and may carry **account risks**. Use responsibly and at your own discretion.

---

## 📜 Features

- ✅ Ultra-fast clicking on the **daily sign-in** button  
- 🔁 Infinite click loop until stopped manually  
- 💰 Periodic balance checks from OpenVerse API  
- 🧠 Prevents links from opening in new tabs (`target="_blank"` removed)  
- 🛑 Graceful stop function with `stopClicker()`

---

## ⚙️ Configuration

The `config` object allows customization:

```js
const config = {
    buttonSelector: '#daiy_sign > div > div > div > div.col.col-9 > div.flex > span > button', // Update if page structure changes
    preventNewTab: true,      // Prevent new tab opening
    balanceCheckFrequency: 500, // Check balance after every N clicks
    tokenLocalStorageKey: 'token' // Token key stored in localStorage
};
```

## 🚀 How to Use

- Open the OpenVerse site and log in.
- Open Developer Console (F12 or Ctrl + Shift + I).
- Paste the script into the Console tab and press Enter.
- The script will start auto-clicking and periodically checking your balance.
To stop it manually, type:

```js
stopClicker()
```
