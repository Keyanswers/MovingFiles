---
title: "File Merger and Organizer in Python"
author: "Juan Carlos Rubio Polania"
date: "2024-11-24"
output: html_document
---

# File Merger and Organizer in Python 📂🐍

## Overview

This script provides a simple workflow for moving and organizing files from multiple folders into a single destination directory using Python.

The code was designed to automatically collect files from different directories and centralize them into one folder for later inspection, validation, or processing.

In this example, image and text files are moved from:
- `BB_images`
- `BB_text`

into a new directory called:
- `CheckingFiles`

Although the example uses image and text folders, the workflow can be adapted to:
- Dataset organization
- Annotation review
- Backup workflows
- File consolidation
- Data preprocessing
- Deep learning pipelines
- General file management

---

# Features

- 📂 Automatic file organization
- 🚚 File transfer between folders
- ⚡ Fast batch processing
- 🐍 Simple Python workflow
- 📁 Automatic directory creation
- 💻 Compatible with multiple file types

---

# Required Packages

The script uses only Python standard libraries:

```python
import os
import shutil
```

No additional installations are required.

---

# Workflow

## 1. Define Main Directory

```python
Path = "C:/Users/ProjectFolder"
```

The main working directory is defined.

---

## 2. Define Source Folders

```python
imapath = os.path.join(Path, "BB_images")
textpath = os.path.join(Path, "BB_text")
```

The script identifies folders containing files to be moved.

---

## 3. Define Destination Folder

```python
DestPath = os.path.join(Path, "CheckingFiles")
```

All files will be transferred into this folder.

---

## 4. Create Destination Directory

```python
os.makedirs(DestPath)
```

The destination folder is automatically created if it does not already exist.

---

## 5. Move Files

```python
shutil.move(FilePath, dest_path)
```

Each file is moved from the source folder into the destination directory.

---

# Example Console Output

```text
Moving files from 'images' folder...
Moved: image1.jpg to CheckingFiles

Moving files from 'text' folder...
Moved: file1.txt to CheckingFiles

All files were moved successfully!
```

---

# Applications

This workflow can be useful for:

- 🧠 Deep learning datasets
- 🖼️ Annotation checking
- 📊 Data preprocessing
- 📂 File organization
- 🛰️ Remote sensing workflows
- 🌿 Ecological datasets
- 💾 Backup automation
- ⚡ Batch file management

---

# Requirements

- Python 3.x

---

# License

This project is licensed under the MIT License.

---

# Author

Juan Carlos Rubio Polania
