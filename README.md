# 📸 Photo Backup Automation Toolkit

A simple, cross-platform script collection to safely and efficiently back up your cloud-based photo libraries to an external hard drive.

This toolkit includes **four automation scripts** (Mac & Windows) — two for copying only, and two for copying *and then deleting* original files to free up cloud storage.

---

## ✅ Features

- Works on **macOS** and **Windows**
- Supports both **iCloud**, **Google Drive**, **OneDrive**, and other cloud sync folders
- **Copy-only** or **copy-and-delete** versions available
- Simple, fast, and safe backup process
- Includes log tracking for every backup

---

## 📁 Script Overview

| Platform | Action        | File                          | Description                            |
|----------|---------------|-------------------------------|----------------------------------------|
| Mac      | Copy Only     | `mac/copy_only.sh`            | Backs up photos without deleting source |
| Mac      | Copy + Delete | `mac/copy_and_delete.sh`      | Backs up photos and clears originals    |
| Windows  | Copy Only     | `windows/copy_only.bat`       | Copies photos to external drive         |
| Windows  | Copy + Delete | `windows/copy_and_delete.bat` | Copies photos and removes source files |

---

## ⚙️ Setup Instructions

### 🔧 Step 1: Customize Paths

Edit each script’s `SOURCE` and `DEST` variables to match your environment:

- `SOURCE`: the folder where your cloud photos are stored locally  
- `DEST`: the folder on your external hard drive where you want them backed up  

### 🍏 Mac Users

- Use `chmod +x script.sh` to make scripts executable
- You can run via Terminal or use Automator to trigger with a click

### 🪟 Windows Users

- Double-click `.bat` files to run
- Scripts will open a console window and display progress
- Make sure your external drive is assigned the correct drive letter (e.g., `E:`)

---

## 🧠 Best Practices

- Always **verify** backups before using the delete versions
- Store your backups in a dated folder structure for easier retrieval
- Review the generated `backup-log.txt` file for audit history

---

## ⚠️ Safety Notes

- These scripts use `xcopy` (Windows) and `cp` (Mac) to mirror your photo directory  
- Deletion only occurs after a successful copy  
- Still, use at your own risk. Always confirm file transfers manually the first time

---

## 🕒 Coming Soon

- Scheduled backup integration (Task Scheduler or `launchd`)
- Support for cloud APIs (Google Takeout, iCloud CLI)
- GUI version

---

## 📬 Support or Contributions

Open an issue or submit a pull request if you’d like to enhance the scripts. This toolkit is designed to be as lightweight and user-controlled as possible.

---

**Made with care to preserve your memories and reclaim your cloud space.**


