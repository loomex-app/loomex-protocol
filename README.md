# loomex-protocol

Versioned, transport-neutral contracts shared by Loomex runtimes.

This crate owns runner identity, surface (`desktop` or `plugin`), platform
metadata, protocol versioning, and compatibility checks. It intentionally does
not contain Tauri, MCP, filesystem, process, or authentication code.

The first supported wire contract is `runner.v1`. Consumers should depend on a
released crate version and use the compatibility helpers during handshake.
