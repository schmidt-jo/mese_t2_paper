# Q2 Visualizations Repository with Git LFS

This repository uses Git Large File Storage (LFS) to manage large movie files in the `data` directory.

## Setup Instructions

### 1. Install Git LFS

Before cloning this repository, you need to install Git LFS:

**For Ubuntu/Debian:**
```bash
sudo apt-get install git-lfs
```

**For macOS (using Homebrew):**
```bash
brew install git-lfs
```

**For Windows (using Chocolatey):**
```bash
choco install git-lfs
```

**For other platforms or manual installation:**
Visit https://git-lfs.github.com/ for installation instructions.

### 2. Clone the Repository

After installing Git LFS, clone this repository:
```bash
git clone <repository-url>
cd <repository-name>
```

### 3. Enable Git LFS for Your User

Initialize Git LFS:
```bash
git lfs install
```

## Working with Large Files

### Adding New Large Files

1. Place your large files in the `data` directory
2. Add and commit as usual:
```bash
git add data/your-large-file.mp4
git commit -m "Add new movie file"
git push
```

### Downloading Large Files

When you clone or pull this repository with Git LFS installed, large files will be automatically downloaded as needed.

If you want to fetch all LFS files:
```bash
git lfs fetch --all
```

## Notes

- Do not modify the `.gitattributes` file unless you know what you're doing
- Always make sure Git LFS is installed before working with this repository
- Large files stored with Git LFS count towards your Git LFS storage quota
