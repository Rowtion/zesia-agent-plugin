# ZESIA Consult

Request an independent review in a local Agent session. ZESIA prepares materials locally and opens the shared browser review. You choose whether to send the displayed materials.

## Set up the local Runtime

This package pins Runtime `0.4.14` for macOS (arm64, x64), Linux (arm64, x64) and Windows (x64).
Install the Skill through your client. Then download [official Setup 1.1.0](https://github.com/Rowtion/zesia-skill/releases/tag/setup-v1.1.0).
Choose the package for your local OS/CPU or the small Node script package if you already have Node 20+.
Verify the asset’s SHA-256 against the checksum on the official release, inspect and extract the ZIP.
Run Setup with the installed path of `skills/zesia-consult` (the directory containing `SKILL.md`).

```text
<setup-node> <path-to-zesia-setup.mjs> agent-plugin "<installed-skill-directory>" --locale <zh-or-en>
```

The platform Setup ZIP includes its private Node executable. Use the verified executable beside the Setup script.
Setup validates the pinned Runtime, installs or reuses it in your user directory, and opens https://zesia.dev/consult for first use.
The Agent and browser must be on the same computer and the Agent must be able to run local commands.

The browser displays exactly what would be sent. The Runtime sends only after your approval and returns the opinion to your agent.
