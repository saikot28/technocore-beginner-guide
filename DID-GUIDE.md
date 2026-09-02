# DID Guide for Beginners

## Introduction

A Decentralized Identifier (DID) is a decentralized identifier that can be used to represent an identity.

DIDs can be useful for applications where users, developers, or AI agents need a persistent and verifiable identity.

## Basic DID Structure

A DID commonly looks like:

```text
did:key:z6Mk...
```

The exact format depends on the DID method.

## Public DID

A public DID can be shared publicly.

For example:

```text
did:key:z6MkExample...
```

A public DID can be used to identify an entity or associate public records with an identity.

## Private Keys

The private key associated with an identity must remain secret.

Never publish:

* Private keys
* Seed phrases
* Passwords
* Secret keys
* API credentials
* Private identity files

Anyone who gains access to private key material may be able to control the associated identity.

## DID and Digital Signatures

DIDs can be used together with cryptographic signatures.

A simplified process is:

```text
Message
   ↓
Private Key
   ↓
Digital Signature
   ↓
Verification
   ↓
Public DID
```

The signature allows another party to verify that the message was signed by the holder of the corresponding private key.

## DID for AI Agents

AI agents may benefit from decentralized identity when they need to:

* Identify themselves
* Sign messages
* Establish trust
* Create verifiable records
* Associate contributions with an identity

## Example Workflow

```text
Generate Identity
       ↓
Obtain Public DID
       ↓
Create Content or Contribution
       ↓
Sign or Record the Contribution
       ↓
Publish the Result
       ↓
Verify the Identity
```

## Security Checklist

Before publishing a project:

* [ ] Check that no private key is included
* [ ] Check that no seed phrase is included
* [ ] Check that no password is included
* [ ] Check that no API secret is included
* [ ] Only publish information intended to be public

## Conclusion

DIDs provide a decentralized approach to digital identity.

For developers and AI-agent applications, they can provide a useful foundation for identity, signatures, and verifiable interactions.
