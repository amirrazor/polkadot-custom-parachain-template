# polkadot-custom-parachain-template
This repository contains a custom Substrate-based parachain template. It has been modified to include additional functionality and serves as a starting point for developers building their own parachains on the Polkadot ecosystem.

---

## Features
- Built with the Polkadot SDK.
- Compatible with Substrate and Polkadot Relay Chain.
- Includes custom runtime and pallet modifications.
- Pre-configured for local development using Zombienet.

---

## Prerequisites
Before running this parachain, make sure the following tools are installed:
- [Rust](https://www.rust-lang.org/) (including `wasm32-unknown-unknown` target)
- [Zombienet](https://github.com/paritytech/zombienet)
- Node.js and npm
- Polkadot Relay Chain Binary

---

## Installation

1. **Clone the Repository**:
   ```
   git clone https://github.com/<your-username>/custom-parachain-template.git
   cd custom-parachain-template
2. **Build the Parachain Node**:


```
cargo build --release
```
3. **Add the Binary to Your PATH: After building, add the binary to your PATH:**


```
export PATH=./target/release:$PATH
```
4. **Download and Set Up the Polkadot Binary:**

- Download the Polkadot binary from the official releases.
Make the binary executable:

```
chmod +x /path/to/polkadot
```
- Add it to your PATH:


```
export PATH=/path/to/polkadot:$PATH
```
## Running the Local Network
1. Start Zombienet: Start the local relay chain and parachain network using Zombienet:


```
zombienet --provider native spawn ./zombienet.toml
```
2. Interact with the Chain:

- Use Polkadot.js Apps to connect to your local network.
- Test functionality using pre-funded accounts.

## License
This project is licensed under the Unlicense.
