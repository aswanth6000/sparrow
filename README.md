# 🕊️ Sparrow

**Sparrow** is a privacy-focused and productivity-first desktop mail client, inspired by Thunderbird — built with modern technologies like [Tauri](https://tauri.app/), [React](https://reactjs.org/), and a monorepo architecture powered by [pnpm](https://pnpm.io/) and [Turborepo](https://turbo.build/).

---

## ✨ Features

* 🔡️ Built with privacy by design.
* ⚡️ Lightning-fast performance using Rust (via Tauri).
* 🧹 Modular monorepo architecture.
* 🎨 Custom UI components via internal shared packages.
* 🌐 Cross-platform support: Windows, macOS, and Linux.

---

## 🧱 Tech Stack

| Layer         | Tech                           |
| ------------- | ------------------------------ |
| Frontend      | React + TypeScript + Vite      |
| Desktop Shell | Tauri (Rust)                   |
| Package Mgmt  | pnpm + Turborepo               |
| Shared Code   | Monorepo: `apps/`, `packages/` |
| Styling (opt) | Tailwind CSS / Native CSS      |

---

## 📁 Folder Structure

```bash
sparrow/
├── apps/
│   ├── desktop/        # Main desktop app (Tauri + React)
│   └── ...             # Other apps
├── packages/
│   ├── core/           # Business logic, email utils, encryption etc.
│   └── ui/             # Shared UI components
└── pnpm-workspace.yaml
    turbo.json
```

---

## 🚀 Getting Started

### Prerequisites

* [Node.js](https://nodejs.org/) (v18+ recommended)
* [Rust](https://www.rust-lang.org/tools/install)
* [pnpm](https://pnpm.io/installation)

### 1. Clone the repo

```bash
git clone https://github.com/aswanth6000/sparrow.git
cd sparrow
```

### 2. Install dependencies

```bash
pnpm install
```

### 3. Run the desktop app in development mode

```bash
pnpm dev:desktop
```

> This launches the React frontend via Vite and Tauri in dev mode.

---

## 📦 Build for Production

```bash
pnpm build:desktop
```

> This builds both React and the Tauri desktop binary for your OS.

---

## 🔐 Privacy & Security

Sparrow is built with privacy-first principles:

* No telemetry
* Local-first email management
* End-to-end encryption (planned)

---

## 🛃️ Roadmap

* [x] Monorepo setup with Tauri + React
* [ ] IMAP/SMTP Email sync
* [ ] End-to-end encryption for emails
* [ ] Offline support
* [ ] Unified search + filtering
* [ ] PGP key integration
* [ ] Cross-device syncing

---

## 🧑‍💻 Contributing

Pull requests are welcome! Please open issues to suggest features or report bugs.

---

## 📄 License

[MIT](./LICENSE)

---

## 🙌 Acknowledgements

* [Tauri](https://tauri.app/)
* [Vite](https://vitejs.dev/)
* [React](https://reactjs.org/)
* [Thunderbird](https://www.thunderbird.net/) – for the inspiration
