# FLOP Devnet & Technocore Beginner Guide

A practical beginner's guide to decentralized agent identity, signed contributions, FLOP Devnet testing, and GPU miner preparation.

**Author:** Saikot  
**Date:** November 5, 2026  
**Technocore DID:** `did:key:z6Mkf2b2ZT9eHNsDNZphE8YrS9ZuMmJGTPbF2xQHYmDbKjU1`

---

## 1. What is Technocore?

Technocore provides public rooms where AI agents and contributors can publish messages associated with cryptographic identities.

A Technocore DID (Decentralized Identifier) allows a contributor to establish a persistent public identity.

The Technocore DID Starter uses Ed25519 cryptography to sign messages.

Repository: https://github.com/zunmax/technocore-did-starter

## 2. My Technocore DID

I created an encrypted Ed25519 identity and successfully loaded my existing identity in Ubuntu on WSL2.

My public DID:

```text
did:key:z6Mkf2b2ZT9eHNsDNZphE8YrS9ZuMmJGTPbF2xQHYmDbKjU1
```

My first signed introduction was successfully published in the `lobby` room.

**Participation record:**

| Field | Value |
|---|---|
| Room | `lobby` |
| Sequence | `147320692` |
| Date | November 5, 2026 |
| DID | My public DID above |
| Status | Successfully posted |

The message:

> Hello from a Technocore contributor. I am building a beginner-friendly guide to Technocore and FLOP Devnet for the community.

A sequence number and signed message provide a public participation record.

## 3. What is FLOP Devnet?

FLOP is developing a decentralized AI compute network.

Devnet provides a development environment for testing network components, AI inference, agents, and miners.

Official resources:

- Explorer: https://explorer.devnet.flop.network
- Faucet: https://faucet.flop.network
- Model API: https://api.flop.network/v1/models
- Hosted MCP: https://mcp.flop.network/mcp

Devnet tokens are experimental and have no real-world monetary value.

## 4. Agent vs. GPU Miner

These are different roles in the network.

### AI Agent

An agent can:
- Request AI model inference.
- Send prompts to compatible miners.
- Receive model responses.
- Use network services and manage its spending.

An agent needs the appropriate wallet, credentials, and network configuration.

### GPU Miner

A miner provides GPU computing resources to serve AI inference workloads.

A miner may need:
- Compatible GPU hardware.
- Docker with NVIDIA GPU support.
- An approved miner package and configuration.
- Operator approval and calibration.
- A reachable endpoint and network connectivity.

Running an agent does not automatically make someone a GPU miner.

## 5. My Devnet Test Balance

I received 25 test FLOP from the Devnet faucet.

These tokens are for testing only.

My planned tests:

1. Check the Devnet wallet balance.
2. Inspect available AI models.
3. Understand inference request costs.
4. Test a small inference request when an approved miner and endpoint are available.
5. Check the resulting usage and transaction records.

I will avoid unnecessary transfers or spending until the test workflow is understood.

**Important:** Test FLOP is not real $FLOP and does not guarantee future token rewards.

## 6. Available AI Model

The Devnet model API previously returned:

```text
qwen/qwen2.5-0.5b-instruct
```

This is a Qwen 2.5 0.5B Instruct model listed for Devnet testing.

Model availability and miner availability are separate. A model appearing in the API does not prove that a specific miner is currently available.

## 7. My GPU Setup

My desktop hardware:

| Component | Specification |
|---|---|
| CPU | Intel Core i5-13400F |
| GPU | NVIDIA GeForce RTX 3060 Ti |
| GPU VRAM | 8 GB |
| RAM | 16 GB |
| OS | Windows 11 + Ubuntu 24.04 WSL2 |
| Container runtime | Docker |

I successfully tested NVIDIA GPU access inside Docker:

```text
CUDA: True
GPU: NVIDIA GeForce RTX 3060 Ti
VRAM: 8.0 GB
```

This confirms that Docker can access my GPU.

However, GPU access alone does not establish miner eligibility. RTX 3060 Ti 8 GB qualification still needs confirmation from FLOP Labs.

## 8. Security Practices

- Never publish `identity.pem`.
- Never share private keys, wallet seed phrases, or passwords.
- Keep the DID public; keep the private key encrypted.
- Verify miner endpoints and approved software before use.
- Use spending limits when making inference requests.
- Do not trust unofficial airdrop or token-claim links.

## 9. My Next Development Goals

- [x] Create a Technocore DID.
- [x] Load the existing DID in WSL Ubuntu.
- [x] Publish a signed introduction in the Technocore lobby.
- [x] Verify Docker GPU access.
- [ ] Publish this beginner guide.
- [ ] Record the guide URL in the Technocore `technocore` room.
- [ ] Check the Devnet wallet balance.
- [ ] Perform a small inference test with an available miner.
- [ ] Obtain confirmation about RTX 3060 Ti miner qualification.
- [ ] Complete miner approval and calibration if eligible.

## 10. Disclaimer

This document records my learning and testing experience with Technocore and FLOP Devnet.

Devnet participation, test tokens, signed messages, and GPU setup do not guarantee an airdrop, token allocation, or financial reward.

Always follow the latest official FLOP Labs instructions.

---

**Learning in public. Building carefully. Verifying every step.**
