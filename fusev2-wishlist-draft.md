# Fuse V2.0 Wishlist

The goal of this document is to have a list of things we wish to do for next five years at Fuse.

Approximate Timeline: 3 months

## Core Ideas & Ambitious Technology Roadmap


## Replacement for openethereum

We need to select a new provider to replace the deprecated openethereum position.

Two potential candidates are:
  Nethermind
  Erigon (The new home of openethereum)

### Benefits of Nethermind:

Built on .Net and c#

    - Plugin Architecture
      >It can dynamically load plugins. It is as simple as dropping dll file into the plugin folder. No need to fork and compile the node yourself. Build once and share with others. No worries about merging multiple forks.
    - MEV Support
      >It has 1st party plugin for MEV compliant with flashbotsmev spec. They will keep supporting future MEV specs directly.
    - Account Abstraction EIP-4337
      It has 1st party AA plugin developed was driven by Kristof Gazso (core author of the EIP).
    - Faster Sync using Snap Sync Mode
      It can use Snap Sync mode to sync the whole Eth1 chain in less than 3 hours.
    - Multi-chain Support
      It has multi-chain support. Apart from mainnet and various testnets, it supports gnosischain and energywebx chain. Both running on AuRa or its extension POSDAO consensus algorithms. It will also support Gnosis merge transition.
    - Fast and Rich JSON RPC Implementation
      It has fast and rich JSON RPC implementation because of partly due to .Net core and some crazy optimizations at some calls like eth_getLogs.
    - Native Blockscout Support for open-source block explorer
      It has native support for block explorer like blockscout.
    - Full support for Eth merge
      It supports Ethereum merge.
    - Native support for monitoring stack
      It has support for monitoring stack using grafana and seq as well as HealthCheck plugin.
    - Supports Full Pruning
      It supports pruning State data directly from disk without stopping the node called (Full Pruning).
    - Support for L2 rollups
      It already supports Starknet L2 client implementation (Juno).
      More support for other L2 rollups in the pipeline
