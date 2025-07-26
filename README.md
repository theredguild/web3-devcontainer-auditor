# Web3 DevContainer - Auditor

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&template_repository=theredguild/web3-devcontainer-auditor)
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/theredguild/web3-devcontainer-auditor)

## What is this?

A forensic-grade security analysis environment for read-only contract examination and vulnerability research. Maintains complete isolation from development activities.

## What's inside?

**Analysis Tools:**
- Slither with full detector suite
- Mythril for symbolic execution
- Manticore for dynamic analysis
- Surya for contract visualization
- Echidna for property-based fuzzing

**Security Features:**
- Complete air-gapping (no network access)
- Read-only workspace (cannot modify source files)
- Tmpfs-only outputs (volatile storage)
- Custom seccomp profile blocks dangerous operations
- Ultra-restrictive container permissions

**Professional Features:**
- Pre-configured audit workflows
- Report generation templates
- Visual analysis capabilities
- One-click comprehensive analysis scripts

## When to use this?

- Professional security audits
- Code reviews for audit firms
- Vulnerability research and analysis
- Academic security research
- Bug bounty hunting
- Post-incident forensic analysis

## How to use?

Click a badge above to launch instantly, or clone this repo and open in VS Code with the Dev Containers extension.

Quick analysis workflow:
```bash
# Comprehensive analysis
/tmp/audit-tools/quick-analysis.sh

# Individual tools
slither . --print human-summary
myth analyze contract.sol
surya inheritance contract.sol | dot -Tpng > /tmp/inheritance.png
```

**Important:** This environment is read-only. All analysis outputs are stored in `/tmp/` and are ephemeral.

## Need something different?

Check the [Web3 DevContainer Hub](https://github.com/theredguild/web3-devcontainer-hub) for development, hardened, or maximum isolation environments.