# Maybe Don't — Downloads

  > Your AI agent wanted to do something. Maybe it shouldn't.

  **Maybe Don't** is a security gateway that sits between AI agents and MCP servers, validating every tool call before it happens. Deterministic CEL policies catch the obvious stuff.
  AI-powered rules catch the rest.

  ## Install

  ### Homebrew (macOS & Linux)

  ```bash
  brew install maybedont/tap/maybe-dont
  ```

  ### Docker

  ```bash
  docker pull ghcr.io/maybedont/maybe-dont:latest
  ```

  ### Binary Download

  Download the latest release from the [Releases](https://github.com/maybedont/releases/releases/latest) page.

  | Platform | Architecture | Download |
  |----------|-------------|----------|
  | macOS | Apple Silicon (arm64) | [tar.gz](https://github.com/maybedont/releases/releases/latest/download/maybe-dont_darwin_arm64.tar.gz) |
  | macOS | Intel (x86_64) | [tar.gz](https://github.com/maybedont/releases/releases/latest/download/maybe-dont_darwin_x86_64.tar.gz) |
  | Linux | arm64 | [tar.gz](https://github.com/maybedont/releases/releases/latest/download/maybe-dont_linux_arm64.tar.gz) |
  | Linux | x86_64 | [tar.gz](https://github.com/maybedont/releases/releases/latest/download/maybe-dont_linux_x86_64.tar.gz) |
  | Windows | arm64 | [zip](https://github.com/maybedont/releases/releases/latest/download/maybe-dont_windows_arm64.zip) |
  | Windows | x86_64 | [zip](https://github.com/maybedont/releases/releases/latest/download/maybe-dont_windows_x86_64.zip) |

  > **Note:** The download links above point to the latest release. For a specific version, browse the [releases page](https://github.com/maybedont/releases/releases) directly.

  ### Verify Your Download

  Every release artifact includes a `.sha256` checksum file. To verify:

  ```bash
  # Download the binary and its checksum
  curl -LO https://github.com/maybedont/releases/releases/latest/download/maybe-dont_darwin_arm64.tar.gz
  curl -LO https://github.com/maybedont/releases/releases/latest/download/maybe-dont_darwin_arm64.tar.gz.sha256

  # Verify
  sha256sum -c maybe-dont_darwin_arm64.tar.gz.sha256
  ```

  ## Quick Start

  ```bash
  # Start the gateway — config is generated on first run
  maybe-dont start

  # Check the version
  maybe-dont version
  ```

  On first run, default configuration files are written to `~/.config/maybe-dont/`. Customize them, then restart.

  ## Documentation

  Full documentation is available at [maybedont.ai/docs](https://maybedont.ai/docs).

  ## License

  © 2025 Maybe Don't, Inc. All rights reserved.
