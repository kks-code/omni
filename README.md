<h1 align="center">Omni Monorepo</h1>

<p align="center">
  <a href="https://docs.omni.network/">
    <img src="https://img.shields.io/badge/Docs-docs.omni.network-176CFF.svg" alt="Docs">
  </a>
  <a href="https://github.com/omni-network/omni/releases/">
    <img src="https://img.shields.io/github/release/omni-network/omni.svg?color=176CFF" alt="Release">
  </a>
  <a href="https://goreportcard.com/report/github.com/omni-network/omni">
    <img src="https://goreportcard.com/badge/github.com/omni-network/omni" alt="Go Report">
  </a>
  <a href="https://github.com/omni-network/omni/actions?query=workflow%3Aci-main">
    <img src="https://img.shields.io/github/actions/workflow/status/omni-network/omni/ci-main.yaml?label=Tests&logoColor=white" alt="Tests">
  </a>
  <a href="https://x.com/OmniFDN">
    <img src="https://img.shields.io/twitter/follow/OmniFDN.svg?label=Follow" alt="Follow">
  </a>
  <a href="https://deepwiki.com/omni-network/omni">
    <img src="https://img.shields.io/badge/DeepWiki-View%20on%20DeepWiki-8A2BE2.svg" alt="DeepWiki">
  </a>
</p>

<div align="center">
  <img src="https://docs.omni.network/img/omni-banner.png" alt="Logo">
</div>

## About Omni

This monorepo contains all source code for the Omni protocol. Omni's goal is to make it easy for smart contract developers to source liquidity and users from anywhere. The protocol consists of various components including an EVM and cross-chain messaging.

The [Omni Docs](https://docs.omni.network/) are the best place to get started learning about Omni. Our [DeepWiki page](https://deepwiki.com/omni-network/omni) is a great place to learn about the structure of this monorepo and Omni's architecture.

## Quickstart

Ensure [go](https://go.dev/doc/install), [goreleaser](https://goreleaser.com/install/) and [docker](https://docs.docker.com/engine/install/) are installed.

```bash
# Build local docker containers
make build-docker

# Run the end-to-end tests on a local devnet
MANIFEST=devnet1 make e2e-run

# Start a local devnet
make devnet-deploy

# Stop the local devnet
make devnet-clean
