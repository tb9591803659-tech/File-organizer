# File Organizer

A lightweight Python utility that automatically organizes clutter in any directory by sorting files into subfolders based on their file extensions.

---

## Features

* **Automatic Detection:** Identifies file types instantly by extension.
* **Auto-Folder Generation:** Creates category folders on the fly if they don't already exist.
* **Clear Feedback:** Displays real-time file-moving actions and a final count of organized files.
* **Zero Dependencies:** Built entirely with Python's standard library.

---

## Supported File Types

| Category | Extensions |
| :--- | :--- |
| **Images** | `.jpg`, `.jpeg`, `.png`, `.gif`, `.svg`, `.webp` |
| **Videos** | `.mp4`, `.mkv`, `.avi`, `.mov` |
| **Audio** | `.mp3`, `.wav`, `.aac`, `.flac` |
| **Documents** | `.pdf`, `.doc`, `.docx`, `.txt`, `.pptx`, `.xlsx`, `.csv` |
| **Programming**| `.py`, `.java`, `.c`, `.cpp`, `.js`, `.html`, `.css` |
| **Archives** | `.zip`, `.rar`, `.7z`, `.tar` |
| **Executables**| `.exe`, `.msi`, `.apk` |
| **Fonts** | `.ttf`, `.otf` |
| **3D Models** | `.obj`, `.stl`, `.fbx` |

---

## Requirements

* Python 3.x
* No external packages required (uses built-in `os`, `shutil`, and `pathlib`).

---

## Installation

Clone the repository:

```bash
git clone [https://github.com/](https://github.com/)<your-username>/file-organizer.git
cd file-organizer
```

# How to Use File Organizer

A step-by-step guide to running and using the File Organizer script on Windows, macOS, and Linux.

---

## 1. Prerequisites

Make sure you have **Python 3.6 or higher** installed.

Check your Python version by running:

```bash
python --version
# or on macOS/Linux:
python3 --version
```

## 2. Setup

clone or download this repository :
```bash
git clone [https://github.com/](https://github.com/)<your-username>/file-organizer.git
cd file-organizer
```

verify the project structure :
```text
file-organizer/
├── src/
│   └── file_organizer.py
└── README.md
```

## 3. Running the Script

Open your terminal or command prompt inside the project folder and run:

### Windows 
```bash
python src/file_organizer.py
```

### Linux
```bash
python3 src/file_organizer.py
```

## 4.Entering directory paths

When prompted with Enter path:, provide the absolute path to the directory you want to organize.

```bash
Enter path: C:\Users\YourUsername\Downloads
Enter path: C:\Users\YourUsername\Desktop\MessyFolder
```

# 5. Final Results
The script validates the path to ensure the folder exists.

It loops through all individual files in the target folder.

Matching category folders (e.g., Images/, Documents/) are created automatically if they don't already exist.

Each file is moved to its corresponding folder, printing its progress in real time:

```text
Moving photo.jpg -> Images/photo.jpg
Moving notes.pdf -> Documents/notes.pdf
Moving script.py -> Programming/script.py

Organization complete! Organized 3 files.
```

Files with unrecognized extensions remain untouched in the root directory.

## 🚀 Future Improvements

Planned enhancements and feature roadmap for upcoming releases:

- [ ] **Graphical User Interface (GUI):** Add a desktop interface using `Tkinter` or `PyQt` for easier non-terminal use.
- [ ] **Command-Line Arguments:** Support CLI flags via `argparse` (e.g., `python file_organizer.py --path /path/to/folder --dry-run`).
- [ ] **Dry-Run / Preview Mode:** Allow users to simulate the process and view proposed moves before executing them.
- [ ] **Recursive Subfolder Sorting:** Add an option to scan nested subdirectories rather than just the top-level folder.
- [ ] **Duplicate File Handling:** Auto-rename files (e.g., `file (1).png`) or compare hashes instead of overwriting.
- [ ] **Custom Configuration:** Allow users to define custom categories and extension mappings via a `config.json` or `.yaml` file.
- [ ] **Activity Logging:** Generate a `cleanup.log` file detailing timestamps, moved files, and errors.
- [ ] **Undo Operation:** Store the last operation state to allow reverting moved files back to their original locations.

---

## 📄 License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for more information.

```text
MIT License

Copyright (c) 2026 Your Name

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```