# cli-prebuilts

Recommended CLI prebuilt binaries which are up-to-date (checked daily).

## Quick Installation

### Prerequisites

Install Git LFS (Large File Storage):

**Ubuntu/Debian:**
```bash
sudo apt update && sudo apt install git-lfs
```

**CentOS/RHEL/Fedora:**
```bash
sudo yum install git-lfs  # CentOS/RHEL
# or
sudo dnf install git-lfs  # Fedora
```

**macOS:**
```bash
brew install git-lfs
```

### Fast Clone & Setup

```bash
# Initialize git-lfs (one-time setup)
git lfs install

# Clone repository (fast - no large files downloaded initially)
git clone https://github.com/ShangjinTang/cli-prebuilts.git ~/.prebuilts

# Enter directory
cd ~/.prebuilts

# Download all binaries from LFS
git lfs pull

# Add to PATH
echo 'export PATH="$HOME/.prebuilts/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## Usage

After installation, all binaries will be available in your PATH:
```bash
bat --help
fd --help
rg --help
nvim --version
```

## Repository Features

- **Fast Clone**: Repository clones quickly without downloading large binaries initially
- **LFS Tracked**: All 26+ binaries are stored efficiently using Git LFS
- **Daily Updates**: Automatically updated with latest releases from GitHub
- **Single Command**: `git lfs pull` downloads all binaries when needed

## For Developers

The repository is optimized for fast operations:
- `git clone` is fast (no large file downloads)
- `git pull` updates metadata quickly  
- `git lfs pull` downloads only binary updates when needed
- All binaries under `bin/` are properly LFS tracked