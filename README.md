# Ready-to-Run .qcow2 Images for Limbo PC Emulator

Welcome! This repository is a curated collection of pre-configured operating systems packaged as `.qcow2` virtual disks. They are specifically optimized to run smoothly on mobile hardware using the **Limbo PC Emulator** (Android) or standard desktop QEMU.

Instead of spending hours wrestling with slow installers, you can just download these images, drop them onto your device, and boot right up.

---

## Available Images (For now) (No Images Are Available rn)

### 💿 Fedora Core 1 (Yarrow)
* **Architecture:** i386 (Emulated Pentium 3 / x86)
* **Disk Format:** QCOW2 (Dynamic / Expanding up to 5GB)
* **File Size:** ~[] 
* **Credentials:** Username: `root` | Password: `123456`
* 🔗 **[Download Fedora Core 1 Image from Google Drive](PASTE_YOUR_DIRECT_DOWNLOAD_LINK_HERE)**

---

## Optimal Limbo Settings (For Older/Mid-Range Phones)

To get the best performance out of these legacy images on devices like the Lenovo Vibe P1 or similar processors, use the following configuration guidelines in Limbo:

* **CPU Model:** `pentium3` or `qemu32`
* **CPU Cores:** `1` *(Crucial: Multi-core emulation often slows down legacy OS kernels due to thread synchronization overhead)*
* **RAM:** `256MB` to `512MB`
* **VGA Display:** `cirrus` *(Uses less processing power than standard VGA)*
* **Audio:** `None` *(Saves up to 15% CPU overhead)*
* **Network:** `None` *(Turn off unless explicitly testing networking utilities)*
* **Advanced Options:** Enable **High Priority**, **Disable ACPI**, and **Disable HPET** to maximize emulation speed.

---

## How to Use

1. Download the desired `.qcow2` image from the Google Drive link above.
2. Transfer the file to your Android device's internal storage.
3. Open Any Emulator that supports .qcow2 Files
4. Create a new machine configuration.
5. Set up the hardware settings using the **Optimal Settings** guide above.
6. Scroll down to **Hard Disk**, check **HDA**, click the dropdown, choose **Open**, and select your downloaded `.qcow2` file.
7. Click the **Play** button at the top to boot!

---

## Contributing

Got a working, optimized `.qcow2` image of another vintage or lightweight OS (like Windows 98, Damn Small Linux, or MS-DOS)? Feel free to open an issue or submit a pull request with your configuration details and host link so we can add it to the repository!

---

## License

This repository and its documentation are licensed under the **MIT License**.

*Disclaimer: The guest operating systems themselves (such as Fedora Core 1) remain governed by their own original open-source licenses (GNU GPL, etc.). The MIT license applies specifically to the virtual machine configurations, optimization guides, and structural packaging provided in this repository.*
