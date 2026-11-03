<div align="center">

# Carl OpenLab

Developer tools built in the open — native desktop apps, npm libraries, and local-first tooling for AI coding agents.

</div>

---

## AI & agent tooling

Software that runs on your machine, against the agents you already have installed.

| Project | What it is |
| --- | --- |
| **[Open Chat](https://github.com/CarlOpenLab/open-chat)** | One workspace for the AI agents already on your machine. Connects Codex, Claude Code, OpenCode, Pi and [ACP](https://agentclientprotocol.com) agents through a local gateway, with conversation history kept in your browser. |
| **[PIM](https://github.com/CarlOpenLab/pim)** | A local-first configuration studio for terminal agent harnesses. Structured forms plus a JSON editor for providers, models, skills, prompt templates and themes — it configures models and never handles your keys, storing only `$VAR` references. |
| **[dsh-acp-hub](https://github.com/CarlOpenLab/dsh-acp-hub)** | ACP agent integration for native DSH Web sessions — provider selection and tool cards. |

## Desktop apps

Native-first software, built in Go with [MyGo](https://mygo.egoist.dev/) or straight Win32 — no Electron.

| Project | What it is |
| --- | --- |
| **[Gloss](https://github.com/CarlOpenLab/Gloss)** | A Git client built for reviewing changes. A pre-flight AI risk scan anchors findings to file and line, a fork-style topology graph shows the branch shape, and staged diffs become Conventional Commits. Pure Go, GPU-rendered, ~20 MB. macOS · Windows · Linux. |
| **[Beacon](https://github.com/CarlOpenLab/beacon)** | An ambient terminal hub that signals when it needs you. Real PTY sessions are shared across the native desktop app, browser and phone through a relay; machines dial out, so there is no port forwarding, dynamic DNS or VPN. |
| **[Muse](https://github.com/CarlOpenLab/muse)** | A WYSIWYG Markdown editor with a tool-using AI writing agent. The window, file tree, outline, editor and agent panel are drawn by Go on the GPU; Markdown renders as you type, Mermaid and math included. |
| **[ccmail](https://github.com/CarlOpenLab/ccmail)** | A quiet, focused email client for multiple accounts — Gmail, QQ Mail, 163, 126, Outlook, iCloud or any IMAP/SMTP service in one inbox. Native controls in a single Go binary, with credentials encrypted on disk. |
| **[StickySnap](https://github.com/CarlOpenLab/StickySnap)** | A Snipaste-style screenshot and pin tool for Windows. `F1` captures, `Enter` pins to the desktop, `F3` pins the clipboard, and pins survive reboots. Pure C++/Win32, local-only. |

## Web & mobile apps

| Project | What it is |
| --- | --- |
| **[Homeport](https://github.com/CarlOpenLab/homeport)** | A privacy-first personal navigation workstation with multi-user cloud sync. Local-first and usable offline, deployable to Vercel with Upstash Redis. |
| **[Supei](https://github.com/CarlOpenLab/supei)** | An infinite-canvas AI design tool: chat to generate HTML prototypes with live streaming preview, click any element for targeted feedback, compare variants side by side, and export a single-file interactive preview. |
| **[Pace](https://github.com/CarlOpenLab/pace)** | A daily-budget expense tracker for Android and iOS. Your ledger stays on your device; AI is optional and off by default. |

## Libraries

Published on npm under the [`@cc-heart`](https://www.npmjs.com/search?q=%40cc-heart) scope. ESM + CJS dual builds with full TypeScript types.

**The `utils` family** — one API surface per runtime:

| Package | Runtime | Covers |
| --- | --- | --- |
| [`@cc-heart/utils`](https://github.com/CarlOpenLab/utils) | environment-agnostic core | shared primitives |
| [`@cc-heart/utils-client`](https://github.com/CarlOpenLab/utils-client) | browser | DOM, clipboard, an rAF scheduler, fetch-based requests, SCSS kit |
| [`@cc-heart/utils-service`](https://github.com/CarlOpenLab/utils-service) | Node.js | fs, path, package and validation helpers |

**More:**

| Package | What it does |
| --- | --- |
| [`@cc-heart/object-to-declare`](https://github.com/CarlOpenLab/object-to-declare) | Generates TypeScript type declarations from JavaScript objects or arrays of objects. |
| [`@cc-heart/electron-use-ipc`](https://github.com/CarlOpenLab/electron-use-ipc) | Type-safe IPC for Electron — declare the contract once and every argument, return value and event payload is inferred across main, preload and renderer. Zero runtime dependencies. |
| [`@cc-heart/storage-cache`](https://github.com/CarlOpenLab/storage-cache) | `localStorage` / `sessionStorage` with namespace isolation and per-entry expiration. |
| [`@cc-heart/vite-plugin-uni-pages-to-enum`](https://github.com/CarlOpenLab/vite-plugin-uni-pages-to-enum) | Vite plugin that turns a uni-app `pages.json` into a route enum, so navigation paths are checked at compile time. |
| [`@cc-heart/eslint-config`](https://github.com/CarlOpenLab/eslint-config) | Shared ESLint config for TypeScript and Vue projects. |

---

## Contributing

Bug reports and pull requests are welcome on any repository. Start with [CONTRIBUTING.md](https://github.com/CarlOpenLab/.github/blob/main/CONTRIBUTING.md), and please follow our [Code of Conduct](https://github.com/CarlOpenLab/.github/blob/main/CODE_OF_CONDUCT.md).

Found a security problem? Please report it privately rather than in a public issue — see [SECURITY.md](https://github.com/CarlOpenLab/.github/blob/main/SECURITY.md).
