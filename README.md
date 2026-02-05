# 🧹 Clear Clutter – Python File Organizer

## 📌 Overview

Clear Clutter is a Python automation script that helps organize files inside a folder by:

* Filtering files by extension (e.g., `.jpg`)
* Renaming files sequentially (`1.jpg`, `2.jpg`, `3.jpg`, ...)
* Moving renamed files into a destination folder
* Preventing overwriting of existing files

This project demonstrates practical file system automation using Python.

---

## 🚀 Features

✅ Reads files from a source directory
✅ Filters files by extension
✅ Automatically renames files in sequence
✅ Moves files to a destination folder
✅ Handles existing files safely (no overwrite errors)
✅ Can be extended to support multiple file formats

---

## 🛠 Tech Stack

* Python 3
* Built-in `os` module

---

## 📂 Project Structure

```
mini_projects/
  clear_clutter/
    test_file/        # Source folder (input files)
    jpg_files/        # Destination folder (renamed output files)
```

---

## ⚙️ How It Works

1. Read all files from source folder
2. Filter only required file types (e.g., `.jpg`)
3. Sort files for consistent numbering
4. Detect existing numbered files in destination folder
5. Start numbering from next available number
6. Rename and move files safely

---

## 🧠 Key Concepts Used

* File handling using `os` module
* Loop-based file processing
* Path management using `os.path.join()`
* Safe folder creation using `os.path.exists()`
* Sequential file naming using counters
* Defensive programming for real-world file systems

---

## ▶️ Usage

### 1️⃣ Set Folder Paths

Update paths in script if needed:

```
mini_projects/clear_clutter/test_file
mini_projects/clear_clutter/jpg_files
```

### 2️⃣ Run Script

```
python clear_clutter.py
```

---

## 💡 Example

### Input (test_file folder)

```
cat.jpg
photo.jpg
dog.jpg
```

### Output (jpg_files folder)

```
1.jpg
2.jpg
3.jpg
```

---

## 🔒 Safety Handling

The script:

* Checks if destination folder exists
* Detects existing numbered files
* Starts renaming from next available number

Prevents:

* File overwrite
* FileExistsError

---

## 📈 Future Improvements

* Support multiple file formats automatically
* Add command line arguments
* Add preview mode (dry run)
* Add logging system
* Convert into reusable Python module

---

## 🎯 Learning Outcomes

Through this project, I learned:

* Practical file automation using Python
* Real-world file system behavior
* Safe scripting practices
* Debugging OS-level errors
* Structuring automation scripts

---

## 📜 License

This project is for learning and educational purposes.

---

## ✨ Author

Developed as part of Python learning and automation practice.
