# OpenCode Copy2 - AI Coding Agent

**AI coding agent, built for the terminal.** A sophisticated monorepo containing multiple interfaces and deployment targets for an intelligent coding assistant.

## 🎯 Core Technology Stack
- **Runtime**: Bun (JavaScript/TypeScript)
- **TUI**: Go (Terminal User Interface)  
- **Web**: Astro (Static Site Generator)
- **Infrastructure**: SST (Serverless Stack)
- **API Generation**: Stainless

## 🔧 Main Components
1. **CLI Tool** (`packages/opencode/`) - Core AI coding agent
2. **Terminal UI** (`packages/tui/`) - Go-based interactive interface  
3. **Web Interface** (`packages/web/`) - Astro-based web app
4. **Cloud Functions** (`packages/function/`) - Serverless backend
5. **Platform Integrations** (`sdks/`) - GitHub Actions & VS Code extensions

## 🧠 Core Agent Architecture
**Core Logic:**
- `provider/` - AI model integrations (OpenAI, Claude, etc.)
- `session/` - Conversation context and agent state management
- `tool/` - Executable functions (file editing, commands, etc.)
- `mcp/` - Model Context Protocol implementation

**Critical Support:**
- `lsp/` - Language Server Protocol for code understanding
- `app/` - Main orchestration and agent workflow
- `file/` - Core file operations

**Infrastructure:**
- `cli/`, `server/` - User interfaces and API layer
- `auth/`, `permission/` - Security and access control
- `storage/`, `snapshot/` - Data persistence and versioning
- `config/`, `global/` - Configuration management
- `installation/`, `trace/`, `util/` - System utilities
- `ide/` - Editor integrations
- `format/` - Code formatting
- `bus/` - Event system coordination

## ⚡ Key Features
- AI-powered terminal coding agent
- Multi-language support (TypeScript, Go)
- IDE integrations (VS Code)
- GitHub Actions integration
- Web interface for management
- Serverless deployment ready

## 📁 Complete Project Structure

```
opencode-copy2/
├── 📁 Root Configuration
│   ├── .editorconfig
│   ├── .gitignore
│   ├── bunfig.toml
│   ├── tsconfig.json
│   ├── opencode.json
│   ├── package.json
│   ├── bun.lock
│   ├── sst.config.ts
│   ├── sst-env.d.ts
│   ├── stainless.yml
│   └── stainless-workspace.json
│
├── 📁 Documentation
│   ├── README.md
│   ├── AGENTS.md
│   ├── STATS.md
│   └── LICENSE
│
├── 📁 Scripts & Installation
│   ├── install (installation script)
│   └── scripts/
│       ├── hooks (bash)
│       ├── hooks.bat (windows)
│       ├── release
│       ├── stainless
│       └── stats.ts
│
├── 📁 GitHub Workflows (.github/)
│   └── workflows/
│       ├── deploy.yml
│       ├── notify-discord.yml
│       ├── opencode.yml
│       ├── publish-github-action.yml
│       ├── publish-vscode.yml
│       ├── publish.yml
│       └── stats.yml
│
├── 📁 Infrastructure (infra/)
│   └── app.ts (SST deployment config)
│
├── 📁 Core Packages (packages/)
│   ├── 📦 opencode/ (Main CLI package - TypeScript/Bun)
│   │   ├── package.json
│   │   ├── bin/ (CLI executables)
│   │   ├── script/ (build scripts)
│   │   ├── test/ (test files)
│   │   └── src/ (Core source code)
│   │       ├── index.ts (main entry)
│   │       ├── app/ (application logic)
│   │       ├── auth/ (authentication)
│   │       ├── bun/ (Bun runtime integration)
│   │       ├── bus/ (event bus)
│   │       ├── cli/ (CLI interface)
│   │       ├── config/ (configuration)
│   │       ├── file/ (file operations)
│   │       ├── flag/ (feature flags)
│   │       ├── format/ (code formatting)
│   │       ├── global/ (global state)
│   │       ├── id/ (ID generation)
│   │       ├── ide/ (IDE integration)
│   │       ├── installation/ (install logic)
│   │       ├── lsp/ (Language Server Protocol)
│   │       ├── mcp/ (Model Context Protocol)
│   │       ├── permission/ (permissions)
│   │       ├── provider/ (AI providers)
│   │       ├── server/ (server logic)
│   │       ├── session/ (session management)
│   │       ├── share/ (sharing functionality)
│   │       ├── snapshot/ (code snapshots)
│   │       ├── storage/ (data storage)
│   │       ├── tool/ (tools integration)
│   │       ├── trace/ (tracing/logging)
│   │       └── util/ (utilities)
│   │
│   ├── 📦 tui/ (Terminal UI - Go)
│   │   ├── go.mod, go.sum
│   │   ├── .goreleaser.yml
│   │   ├── cmd/ (command definitions)
│   │   ├── input/ (input handling)
│   │   ├── internal/ (internal packages)
│   │   └── sdk/ (SDK integration)
│   │
│   ├── 📦 web/ (Web interface - Astro)
│   │   ├── package.json
│   │   ├── astro.config.mjs
│   │   ├── config.mjs
│   │   ├── public/ (static assets)
│   │   └── src/ (web source code)
│   │
│   ├── 📦 function/ (Serverless functions)
│   │   ├── package.json
│   │   └── src/ (function source)
│   │
│   └── 📦 sdk/ (Software Development Kit)
│       └── (SDK code)
│
└── 📁 Platform SDKs (sdks/)
    ├── 📦 github/ (GitHub Action/Integration)
    │   ├── action.yml
    │   ├── package.json
    │   ├── script/ (build scripts)
    │   └── src/ (GitHub integration code)
    │
    └── 📦 vscode/ (VS Code Extension)
        └── (extension code)
```

---

*This is a fork of the OpenCode AI terminal coding agent project.*