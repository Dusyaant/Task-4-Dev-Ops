# 🐚 Shell Scripting Tasks

## 📌 Overview

This repository contains basic shell scripting tasks focused on:

* Checking HTTP status of a website
* Performing conditional text replacement using `sed`

---

## 🚀 Task 1: HTTP Status Checker

This script fetches the HTTP status code of **guvi.in** and prints a success/failure message based on the response.

### ▶️ Run

```bash
bash scripts/check_status.sh
```

### 🧠 Logic

* Uses `curl` to get HTTP status code
* If status code is between **200–399 → Success**
* Otherwise → Failure

### 📷 Output

![HTTP Status Output](screenshots/mv your_image1.png 01-http-status-success.png)

---

## 🛠️ Task 2: Text Processing using sed

This script replaces all occurrences of the word **"give"** with **"learning"**
➡️ From **line 5 to end of file**
➡️ Only in lines containing the word **"welcome"**

### ▶️ Run

```bash
bash scripts/text_replace.sh sample.txt
```

### 🧠 Logic

* Uses `sed` with:

  * Line range: `5,$`
  * Condition: `/welcome/`
  * Replacement: `s/give/learning/g`

### 📷 Output

![Text Processing Output](screenshots/02-sed-text-processing.png)

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

## ⚠️ Notes

* HTTP status **301** indicates a redirect but still considered reachable
* Ensure scripts have execution permission:

```bash
chmod +x scripts/*.sh
```

---

## 🧠 Concepts Used

* Bash scripting
* curl
* sed
* Conditional logic
* File manipulation

---

## 📎 Author

Dusyaant R
