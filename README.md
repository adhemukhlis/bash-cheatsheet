# Bash Command Collection

This repository is a collection of bash/terminal commands for easy reference and quick lookup.

## Table of Contents

### Pinned

- [Disk Usage](#disk-usage)

### Common

- [Disk Usage](#disk-usage)

### Installation

- [NVM](#nvm)
- [Node.js](#node.js)
- [PNPM](#pnpm)

---

## Common

### Disk Usage

```bash
du -h -d 1 | sort -rh
```

---

## Installation

### NVM

[NVM](https://github.com/nvm-sh/nvm) (Node Version Manager) is a tool used to manage and switch between multiple Node.js versions on a single machine.

1. installation
   ```bash
   wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash && source ~/.profile
   ```
   > this command use `v0.40.3`, please check nvm version reference https://github.com/nvm-sh/nvm/releases
2. check version
   ```bash
   nvm --version
   ```

### Node.js

[Node.js](https://nodejs.org) is a cross-platform, open-source JavaScript runtime environment that executes JavaScript code outside a web browser.

1. ensure [NVM](#nvm) is installed
2. node.js version list
   ```bash
   nvm ls-remote
   ```
3. install node.js

   ```bash
   nvm install 24.13.0
   ```

   > this command use `24.13.0` version, please check node.js version reference https://nodejs.org/en/about/previous-releases

   > [!TIP]
   > use `Latest LTS` to install latest long term support version

4. check node.js version
   ```bash
   node --version
   ```

### PNPM

[PNPM](https://pnpm.io) (Package Manager for Node.js) is a tool used to manage and install packages for Node.js projects.

1. enabling corepack
   ```bash
   corepack enable
   ```
   > this command use `corepack`, please check corepack reference https://nodejs.org/api/corepack.html
2. install pnpm

   ```bash
   corepack prepare pnpm@10.28.0 --activate
   ```

   > this command use `10.28.0` version, please check pnpm version reference https://github.com/pnpm/pnpm/releases

   > [!TIP]
   > use `Latest` to install latest version

3. check pnpm version
   ```bash
   pnpm --version
   ```
