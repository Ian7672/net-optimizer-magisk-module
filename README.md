# NetOptimizer

![Magisk](https://img.shields.io/badge/Magisk-Compatible-brightgreen)
![Android](https://img.shields.io/badge/Android-7.0%2B-blue)
![Version](https://img.shields.io/badge/Version-1.0-orange)

NetOptimizer is a Magisk module that optimizes your Android network connection by tweaking TCP/IP and DNS settings. This module aims to improve connection stability, reduce latency, and speed up internet access systematically without modifying system files.

---

## ✨ Key Features

### TCP Optimizations
- Enable TCP Fast Open
- Reuse TIME-WAIT sockets
- Shorten TCP FIN timeout
- TCP window scaling
- Use BBR as congestion control
- Set FQ as default queuing discipline

### DNS Tweaks
- Default using Cloudflare DNS (1.1.1.1 / 1.0.0.1)
- Faster DNS resolution and lower browsing delay

### Systemless & Lightweight
- Does not modify system files
- Can be uninstalled anytime via Magisk Manager

---

## 📥 Installation

1. Download `NetOptimizer.zip`
2. Open Magisk Manager → Modules → Install from storage
3. Select the NetOptimizer.zip file
4. Reboot your device
5. After reboot, TCP BBR and Cloudflare DNS are automatically applied

---

## 📁 Module Structure

```
NetOptimizer/
├─ META-INF/
│   └─ com/google/android/
│       ├─ update-binary
│       └─ updater-script
├─ common/
│   └─ system.prop
├─ service.sh
├─ post-fs-data.sh
├─ module.prop
```

---

## ⚠️ Notes

- This module is fixed default: Cloudflare DNS and TCP BBR are pre-applied
- No manual configuration options
- Safe to use on rooted devices with Magisk

---

## 📋 Compatibility

- Magisk version 24+
- Android 7.0 (Nougat) or higher
- CPU: ARM / ARM64

---

## 📄 License

Free to use, no warranty.

---

## 👨‍💻 Developed by

[github.com/Ian7672](https://github.com/Ian7672)
