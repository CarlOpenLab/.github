<div align="center">

# Carl OpenLab

Developer tools built in the open — npm libraries, desktop apps, and local-first tooling for AI coding agents.

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

| Project | What it is |
| --- | --- |
| **[Muse](https://github.com/CarlOpenLab/muse)** | A WYSIWYG Markdown editor for the desktop. Type `#` and it becomes a heading; code blocks highlight in real time via Shiki. Built on Milkdown 7 with Go (MyGo) + Vue 3. |
| **[Homeport](https://github.com/CarlOpenLab/homeport)** | A privacy-first personal navigation workstation with multi-user cloud sync. Local-first and usable offline, deployable to Vercel with Upstash Redis. |

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
