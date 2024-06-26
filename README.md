# NetWatch

## Wrapper for Android Keystore System

## Project Goal

The main goal of the Netwatch team is to use the advanced security features of the Android platform, namely the Android Keystore system. The Android Keystore system lets you store cryptographic keys in a container to make them more difficult to extract from the device. The Android Keystore API and the underlying Keymaster HAL provide a basic but adequate set of cryptographic primitives to allow the implementation of protocols using access-controlled, hardware-backed keys. Sensitive operations are delegated to a secure processor reached through some kernel interface. The resulting architecture looks like this:

![alt text](static/access-to-keymaster.png)

The goal of the project is to create a Rust-based wrapper that connects the HSM (Android Keystore) with the Crypto-Abstraction Layer provided by [j&s-soft](https://github.com/nmshd), eliminating the complexity of direct communication and provides an API that is secure, effective and developer-friendly.

## Features

- **HSM Wrapper**: A layer that abstracts the complexities of directly interacting with the HSM.
- **Crypto Abstraction Integration**: Integration with j&s-soft's Crypto Abstraction Layer.
- **Dedicated API**: A dedicated API for communicating with the SE/TEE.

## Getting Started

### Prerequisites

- Rust Programming Language: Install the latest version of Rust on your system. You can install Rust through [rustup](https://rustup.rs/).

### Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/netwatch.git
```

2. Navigate to the project directory:

```bash
cd netwatch
```

3. Build the project:

```bash
cargo build
```

## Contributing

We welcome contributions from the community. Please submit a pull request if you detect any bugs, have ideas for enhancements, or would like to add new functionality.

## License

This project is released under the [MIT License](LICENSE).

## Acknowledgments

- Special thanks to [j&s-soft](https://github.com/nmshd) for providing the Crypto Abstraction Layer.
