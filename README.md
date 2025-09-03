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

| Binary | GitHub HomePage | Stars | Last Release | Description |
| --- | --- | --- | --- | --- |
| nvim | [neovim/neovim](https://github.com/neovim/neovim/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/neovim/neovim?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/neovim/neovim?style=flat-square&label=) | |
| mise | [jdx/mise](https://github.com/jdx/mise/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/jdx/mise?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/jdx/mise?style=flat-square&label=) | |
| atuin | [atuinsh/atuin](https://github.com/atuinsh/atuin/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/atuinsh/atuin?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/atuinsh/atuin?style=flat-square&label=) | |
| ast-grep | [ast-grep/ast-grep](https://github.com/ast-grep/ast-grep/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/ast-grep/ast-grep?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/ast-grep/ast-grep?style=flat-square&label=) | |
| bat | [sharkdp/bat](https://github.com/sharkdp/bat/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/sharkdp/bat?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/sharkdp/bat?style=flat-square&label=) | |
| croc | [schollz/croc](https://github.com/schollz/croc/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/schollz/croc?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/schollz/croc?style=flat-square&label=) | |
| csvlens | [YS-L/csvlens](https://github.com/YS-L/csvlens/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/YS-L/csvlens?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/YS-L/csvlens?style=flat-square&label=) | |
| delta | [dandavison/delta](https://github.com/dandavison/delta/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/dandavison/delta?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/dandavison/delta?style=flat-square&label=) | |
| dua | [Byron/dua-cli](https://github.com/Byron/dua-cli/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/Byron/dua-cli?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/Byron/dua-cli?style=flat-square&label=) | |
| dust | [bootandy/dust](https://github.com/bootandy/dust/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/bootandy/dust?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/bootandy/dust?style=flat-square&label=) | |
| eza | [eza-community/eza](https://github.com/eza-community/eza/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/eza-community/eza?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/eza-community/eza?style=flat-square&label=) | |
| fd | [sharkdp/fd](https://github.com/sharkdp/fd/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/sharkdp/fd?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/sharkdp/fd?style=flat-square&label=) | |
| hexyl | [sharkdp/hexyl](https://github.com/sharkdp/hexyl/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/sharkdp/hexyl?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/sharkdp/hexyl?style=flat-square&label=) | |
| hyperfine | [sharkdp/hyperfine](https://github.com/sharkdp/hyperfine/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/sharkdp/hyperfine?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/sharkdp/hyperfine?style=flat-square&label=) | |
| jq | [jqlang/jq](https://github.com/jqlang/jq/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/jqlang/jq?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/jqlang/jq?style=flat-square&label=) | |
| lazygit | [jesseduffield/lazygit](https://github.com/jesseduffield/lazygit/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/jesseduffield/lazygit?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/jesseduffield/lazygit?style=flat-square&label=) | |
| lsd | [lsd-rs/lsd](https://github.com/lsd-rs/lsd/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/lsd-rs/lsd?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/lsd-rs/lsd?style=flat-square&label=) | |
| miniserve | [svenstaro/miniserve](https://github.com/svenstaro/miniserve/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/svenstaro/miniserve?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/svenstaro/miniserve?style=flat-square&label=) | |
| ouch | [ouch-org/ouch](https://github.com/ouch-org/ouch/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/ouch-org/ouch?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/ouch-org/ouch?style=flat-square&label=) | |
| procs | [dalance/procs](https://github.com/dalance/procs/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/dalance/procs?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/dalance/procs?style=flat-square&label=) | |
| rg | [BurntSushi/ripgrep](https://github.com/BurntSushi/ripgrep/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/BurntSushi/ripgrep?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/BurntSushi/ripgrep?style=flat-square&label=) | |
| sad | [ms-jpq/sad](https://github.com/ms-jpq/sad/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/ms-jpq/sad?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/ms-jpq/sad?style=flat-square&label=) | |
| sd | [chmln/sd](https://github.com/chmln/sd/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/chmln/sd?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/chmln/sd?style=flat-square&label=) | |
| tldr | [dbrgn/tealdeer](https://github.com/dbrgn/tealdeer/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/dbrgn/tealdeer?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/dbrgn/tealdeer?style=flat-square&label=) | |
| watchexec | [watchexec/watchexec](https://github.com/watchexec/watchexec/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/watchexec/watchexec?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/watchexec/watchexec?style=flat-square&label=) | |
| yazi | [sxyazi/yazi](https://github.com/sxyazi/yazi/releases/latest) | ![GitHub Repo stars](https://img.shields.io/github/stars/sxyazi/yazi?style=flat-square&label=) | ![GitHub last release](https://img.shields.io/github/release-date/sxyazi/yazi?style=flat-square&label=) | |
