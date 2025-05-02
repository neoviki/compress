# Linux Utility: `compress` and `decompress`

A simple Linux utility to compress and decompress files or directories into the .tar.gz format — using straightforward commands that eliminate the need to remember tar flags or manually set output filenames. Just run the command followed by the folder or archive name.

The goal is to provide a minimal and intuitive way to compress or decompress—just specify the folder or .tar.gz file, with no extra options required.

---

## Features

- Compress files/directories to `.tar.gz`
- Decompress `.tar.gz` archives safely
- Prevents accidental overwrites
- Minimal CLI interface

---

## Install

Run the provided script:

```bash
chmod +x ./install.sh
./install.sh
```

This will install the `compress` and `decompress` utilities to `/usr/local/bin`, making them available system-wide.

---

## Uninstall

To remove the utilities:

```bash
./uninstall.sh
```

---

## Usage

### Compress

```bash
compress <file_or_directory>
```

Creates a `.tar.gz` archive in the current working directory.

**Example:**

```bash
compress my_folder
```

Produces: `my_folder.tar.gz`

> Will not overwrite existing archives with the same name.

---

### Decompress

```bash
decompress <file.tar.gz>
```

Extracts the archive into the current directory.

**Example:**

```bash
decompress my_folder.tar.gz
```

> Will abort if a file or folder with the same name already exists.

---

## Why Use This?

Instead of remembering or typing tar -czf followed by both the directory and the output .tar.gz filename or tar -xzf to extract — just type:

- `compress my_project`
- `decompress my_project.tar.gz`

Quick and Safe.
