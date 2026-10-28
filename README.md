# MyPOS — Downloads

MyPOS is a point-of-sale for shops, marts and stores on Windows. It works **offline**: no internet or cloud account is needed to sell, take returns, manage stock, print receipts or close the day.

## ⬇️ Download

**[Download the latest version](https://github.com/saqlain-codecraf/MyPOS-Release/releases/latest)**

On the release page, under **Assets**, download **`MyPOS-Setup-x.y.z.exe`**. You only need this one file; the others (`latest.yml`, `.blockmap`) are used by automatic updates.

## 💻 System requirements

| | Minimum |
|---|---|
| Windows | Windows 10 or 11, 64-bit |
| Memory | 4 GB RAM |
| Disk | 500 MB free (more for years of sales and backups) |
| Screen | 1280 × 720 or larger |
| Printers | Thermal receipt printers (58 mm or 80 mm) or any Windows printer — optional |
| Scanner | Any USB barcode scanner that types like a keyboard — optional |
| Internet | Only for updates, and to connect several counters through a MyPOS server |

## 🛠️ Install

1. Run **`MyPOS-Setup-x.y.z.exe`**.
2. Windows may show **"Windows protected your PC"** because the installer is not code-signed. Click **More info → Run anyway**.
3. Choose the install folder (or keep the default) and finish the setup. MyPOS appears in the Start menu.

## 🚀 First start

1. Choose **Set up a new business**.
2. Enter your **business name**, country, **currency** and time zone (filled in from Windows), plus address and phone if you like.
3. Name your **store and counter** and pick the **receipt printer**.
4. Turn **tax** on or off and set its rate.
5. Create the **administrator** (username + password of at least 6 characters, and an optional quick PIN). You can add a cashier with a PIN too.
6. Sign in and set up from the back office:
   - **Products** — categories, brands, units, prices, barcodes
   - **Inventory** — opening stock, suppliers and purchases
   - **Users & roles** — staff, PINs and what each role may do
   - **Settings** — receipts, taxes, payment methods, shortcuts, backups

Press **Ctrl + /** on any screen to see the keyboard shortcuts.

## 🖥️ More counters

Each counter is its own PC with MyPOS installed. To share products, stock and reports between counters and stores, they connect through a **MyPOS server**:

| Step | Where |
|---|---|
| Connect the first PC | Back office → **Synchronisation** → Register, with the server address and enrollment code from your provider |
| Add another counter | Install MyPOS, choose **Add this counter to an existing store**, and enter the server address and a join code |

Every counter keeps selling when the internet or server is down, and catches up when it is back.

## 🔄 Updates

- MyPOS checks for a new version in the background when it starts and every few hours, and downloads it quietly.
- When it is ready, a green **Update ready** button appears in the top bar. Click it when convenient — MyPOS backs up your data, closes, updates and opens again in under a minute.
- It **never restarts by itself** during a sale. If you don't click it, the update installs the next time MyPOS is closed.
- You can also check in **Settings → Updates → Check now**.
- Each PC updates itself and needs internet only for the download. Keep all counters on the same version.

## 💾 Your data and backups

All data stays on this PC, in `%APPDATA%\MyPOS\`:

| Folder | What is in it |
|---|---|
| `data` | The database: sales, products, stock, customers, settings |
| `data\backups` | Automatic backups (newest 14 kept), a backup every time MyPOS closes, and one before every update |
| `logs` | Logs for troubleshooting |

- **Updating or uninstalling MyPOS does not delete this folder.**
- When this PC is online, MyPOS sends the business name, phone and address with the app version to its developer — once after setup and then once a month. Sales, stock and customer details are never sent.
- Make extra backups and choose a backup folder (e.g. a USB drive) in **Settings → Backup & account**.
- To move to a new PC, install MyPOS there and choose **Restore from a backup** on the first screen.

## ❓ Troubleshooting

| Problem | What to do |
|---|---|
| "Windows protected your PC" | Click **More info → Run anyway**. |
| Nothing prints | Check the printer is on and selected in **Settings → Printers & devices**, then print a test receipt. |
| Barcode scanner adds nothing | Click the search box on the sale screen and scan again; the scanner must be in keyboard mode. |
| Red bar "This POS will be locked in N days" | Call or WhatsApp **0349 3437606**. |
| "This POS has been locked" | Call or WhatsApp **0349 3437606**, then press **Check again**. Your data is safe on this PC. |
| Forgot the admin password | Another user with the *Manage users* permission can set a new one under **Users**. |

## 📋 Versions

| Version | Date | Notes |
|---|---|---|
| [1.1.0](https://github.com/saqlain-codecraf/MyPOS-Release/releases/tag/v1.1.0) | 28 Oct 2026 | First public release: automatic updates, install report and provider messages (contact 0349 3437606) |

---

© MyPOS. All rights reserved. This repository contains installers only.
