# 🐚 Shell Scripting Automation Tasks

## 📌 Overview

This project demonstrates basic automation using shell scripting.
It includes:

* Checking HTTP status of a website using `curl`
* Performing conditional text processing using `sed`

The goal is to understand real-world scripting concepts like network validation and file manipulation.

---

## 🚀 Task 1: HTTP Status Checker

This script fetches the HTTP status code of **guvi.in** and prints whether the website is reachable.

### ▶️ Run

```bash
bash scripts/check_status.sh
```

### 🧠 How It Works

* Uses `curl` to fetch HTTP status code
* Checks if the code is between **200–399**
* Prints:

  * ✅ Success → Website is reachable
  * ❌ Failure → Website is not reachable

> Note: Status code **301** indicates a redirect but is still considered reachable.

---

## 🛠️ Task 2: Text Processing using sed

This script replaces all occurrences of the word **"give"** with **"learning"**
➡️ From **line 5 onwards**
➡️ Only in lines containing the word **"welcome"**

### ▶️ Run

```bash
bash scripts/text_replace.sh sample.txt
```

### 🧠 How It Works

* Uses `sed` command
* Applies:

  * Line range: `5,$`
  * Condition: `/welcome/`
  * Replacement: `s/give/learning/g`

---

## 📁 Project Structure

```
shell-scripting-tasks/
│
├── scripts/
│   ├── check_status.sh
│   └── text_replace.sh
│
├── screenshots/
│   ├── 01-http-status-success.png
│   └── 02-sed-text-processing.png
│
└── README.md
```

---

## ⚙️ Setup Notes

Before running scripts, ensure execution permission:

```bash
chmod +x scripts/*.sh
```

---

## 🔥 Key Learnings

* Handling HTTP responses using `curl`
* Using `sed` with conditions and line ranges
* Debugging shell script errors
* Understanding environment differences (Ubuntu vs Windows)
* Organizing and documenting a project for GitHub

---

## 📎 Author

Dusyaant R 🚀

