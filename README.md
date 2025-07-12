# 🗃️ Log Archive Tool

A simple Bash-based command-line utility to archive system or application logs into compressed `.tar.gz` files with a timestamp. Useful for system administrators, developers, or anyone managing log directories.

---

## 📦 Features

- Accepts any log directory as input
- Archives all files inside the directory into a timestamped `.tar.gz` file
- Stores archived logs in a dedicated `archives/` folder
- Logs every archive operation with date and time to `archives/archive.log`

---

## 🛠️ Requirements

- Linux or Unix-based system
- Bash shell
- `tar` utility
- `sudo` access (if archiving system directories like `/var/log`)

---

## 🚀 Usage

### 1. Make the script executable

```bash
chmod +x log-archive
```

### 2. Run the tool

```bash
./log-archive <log-directory>
```

### 3. Output
- The archive will be saved in the archives/ folder with a name like:
```
logs_archive_20240712_113015.tar.gz
```

- A log of the operation will be written to:
```
archives/archive.log
```

## 📁 Example Output

```bash
$ sudo ./log-archive /var/log
✅ Archive created: ./archives/logs_archive_20240712_113015.tar.gz
```
