# Outlook Automation

> Automates the running Microsoft Outlook application to manage emails and calendar appointments.

The bundle zip (**29.6 MB**) is stored in this repository at **`e69b6091-4608-4c6c-8c73-3376c354c20a.zip`**.

This repository is part of the **Forjinn-Desk** MCP bundle collection. An MCP bundle is a self-contained server that a host application launches and communicates with over the MCP (Model Context Protocol) protocol.

## Repo metadata

| Field | Value |
| --- | --- |
| Registry ID | `e69b6091-4608-4c6c-8c73-3376c354c20a` |
| Status in registry | inactive |
| Bundle size | 29.6 MB |
| Distribution | committed to this repo |

## Environment variables

| Variable | Value / note |
| --- | --- |
| _(none)_ | _no required environment variables_ |

## MCP launch configuration

The host replaces `__INSTALL_DIR__` (install dir) and `__PYTHON__` (bundled Python) at runtime.

```json
{
  "command": "__PYTHON__",
  "args": [
    "server.py"
  ]
}
```

## Setup / usage notes

Microsoft Outlook must be open and running on the desktop before using this tool. The tool connects to the already-running Outlook instance via COM automation.


## Install / usage

1. Get the bundle:
   - download `e69b6091-4608-4c6c-8c73-3376c354c20a.zip` from this repo (Code → Download ZIP, or `git clone`).
2. Extract to your target installation directory (config paths expect contents at the install-dir root).
3. Set the environment variables listed above.
4. Launch using the MCP config JSON (or let a host client manage it automatically).

> Bundles may include vendored runtimes (bundled Python, Node, or native executables). Builds are Windows x64.
