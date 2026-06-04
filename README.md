# DiskBroom

DiskBroom is a small Python project I built to experiment with Linux disk cleanup tasks. It includes command-line and GTK-based graphical interfaces for inspecting files and running basic cleanup operations.

## Features

- Find duplicate, old, oversized, and temporary files.
- Inspect and clean selected browser and application caches.
- Run basic system cleanup operations, such as package-cache cleanup and trash removal.
- Preview some cleanup operations before deleting files.

## Requirements

- Linux
- Python 3
- `rich` for the command-line interface
- GTK 3 and PyGObject for the graphical interface

## Running

Clone the repository:

```bash
git clone https://github.com/JZX100II/DiskBroom.git
cd DiskBroom
```

Install the command-line dependency:

```bash
pip install rich
```

Run the CLI:

```bash
python3 src/disk_broom.py --help
```

Run the GUI:

```bash
python3 src/disk_broom_gui.py
```

## Notes

This is an experimental project and has not been thoroughly tested. Cleanup operations can delete files, so review the code and inspect the targets before running them. Use dry-run mode where available.