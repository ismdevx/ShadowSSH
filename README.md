<p align="center">
  <img src="public/os-icons/shadowssh-logo.png" alt="ShadowSSH" width="420" />
</p>

<h1 align="center">ShadowSSH</h1>

<p align="center">
  A modern desktop SSH client built with Electron, React, and xterm.js.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="version" />
  <img src="https://img.shields.io/badge/license-MIT-green" alt="license" />
  <img src="https://img.shields.io/badge/platform-Linux%20%7C%20Windows%20%7C%20macOS-lightgrey" alt="platform" />
  <img src="https://img.shields.io/badge/electron-41-47848F?logo=electron" alt="electron" />
</p>

---

## Features

- **Multi-tab SSH sessions** — open multiple connections simultaneously with per-tab status tracking
- **SFTP file browser** — browse, upload, download, and manage remote files with drag-and-drop support
- **Host manager** — save and organize SSH hosts with custom labels and OS icons (20+ distros)
- **SSH key generation** — generate Ed25519/RSA keys directly from the app
- **Jump host / proxy support** — connect through a bastion/jump server
- **Backup & restore** — export and import your saved hosts
- **Config file editor** — edit remote config files in-app
- **Live connection monitor** — view active sessions and their status
- **Auto updates** — automatic update checks via GitHub Releases
- **Themes** — Dark, Light, and Onyx UI themes; 8 terminal color presets (Oceanic, Matrix, Amber, Nord, Dracula, Solarized, and more)
- **OS detection** — auto-detects remote distro and shows the matching icon

---

## Download

Grab the latest release from the [Releases](https://github.com/ismdevx/ShadowSSH/releases) page.

| Platform | Format |
|----------|--------|
| Linux    | `.deb` (Debian/Ubuntu), `.AppImage` |
| Windows  | ⚠️ Currently under development |
| macOS    | `.dmg` |

---

## Install (Linux)

**Debian / Ubuntu / Kali / Mint:**
```bash
sudo dpkg -i shadowssh_1.0.0_amd64.deb
```

**AppImage:**
```bash
chmod +x ShadowSSH-1.0.0.AppImage
./ShadowSSH-1.0.0.AppImage
```

---

## Build from Source

**Prerequisites:** Node.js 20+, npm

```bash
git clone https://github.com/ismdevx/ShadowSSH.git
cd ShadowSSH
npm install
```

**Run in development:**
```bash
npm run dev
```

**Build packages:**
```bash
# Linux (.deb + AppImage)
npm run dist

# macOS (.dmg)
npm run dist:mac
```

Build output lands in `dist-packages/`.

---

## Tech Stack

| Layer     | Technology |
|-----------|-----------|
| Shell     | Electron 41 |
| UI        | React 19 + TypeScript |
| Terminal  | xterm.js 6 |
| Styling   | Tailwind CSS 4 |
| SSH       | ssh2 |
| Bundler   | Vite 8 |

---

## License

MIT © [ismdevx](https://github.com/ismdevx)
