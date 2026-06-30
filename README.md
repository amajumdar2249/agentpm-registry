# 🌌 AgentPM Global Registry

<div align="center">
  <h3><b>The Official Package Registry for Autonomous AI Environments</b></h3>
  <p>Securely hosting 44,500+ production-grade AI skills, tools, and personas.</p>
</div>

---

[![Database Status](https://img.shields.io/badge/Status-Online-brightgreen?style=for-the-badge)](https://github.com/amajumdar2249/agentpm-registry)
[![Packages](https://img.shields.io/badge/Packages-44.5k+-blue.svg?style=for-the-badge)](https://github.com/amajumdar2249/agentpm-registry)
[![Security: Sentinel](https://img.shields.io/badge/Security-Zero%20Trust-red?style=for-the-badge)](https://github.com/amaju/agentpm)

## 📌 What is this Repository?

This is the **Global Raw Database** for the [AgentPM Ecosystem](https://github.com/amajumdar2249/agentpm). 
It serves as the backend infrastructure for the `agentpm install` CLI command. It is not meant to be browsed manually, but rather consumed directly by your AI agents and terminals.

This registry contains massive, cryptographically hashed JSON indexes and raw AST-audited markdown skills that your CLI downloads, parses, and safely injects into `.agents`, `.cursorrules`, or `.windsurf` environments.

## 🚀 How to use it?

You do **not** need to manually download files from here. The `agentpm` CLI interacts with this registry securely.

```bash
# 1. Install the CLI directly from official NPM Registry
npm install -g @amajumdar2249/agentpm

# 2. Search & Install skills (CLI will automatically query this repo)
agentpm install @oss/react-expert
agentpm install karpathy-guidelines
```

## 🔒 Security Architecture

Every package hosted in the `packages/` directory of this registry has passed through a proprietary AST (Abstract Syntax Tree) heuristics audit before being pushed. 

By pulling from this registry, you are guaranteed that the prompt/skill contains:
- `0` Malicious Prompt Injections
- `0` Hidden Data Exfiltration attempts
- `0` AI Jailbreak triggers

## 📂 Repository Structure

- `index.json`: The 13MB+ master database index resolving all packages, dependencies, and versions.
- `packages/`: The physical, raw storage of all 44,562 audited `.md` and `.json` skills.

## 🤝 Contributing
To submit your own skills to the Neural Registry, please read the contribution guidelines in the main [AgentPM Client Repo](https://github.com/amajumdar2249/agentpm). 
