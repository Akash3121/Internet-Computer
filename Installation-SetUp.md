## Setting up the development environment for IC
Local Development Setup

IC SDK is designed to work directly with **Linux or macOS 12**.

To install the Internet Computer Software Development Kit, run:

sh -ci "$(curl -fsSL https://internetcomputer.org/install.sh)"

Check that you have the DFINITY execution command-line interface (CLI) installed and the dfx executable is available in your PATH by running the following command:

dfx --version

## For Windows

Watch this video: https://www.youtube.com/watch?v=ywE2PBNm9Jo

Setup ICP environment with WSL2 Command List (commands used in the above video)

### To download Powershell 1️⃣

PowerShell-7.3.9-win-x64.msi
PowerShell-7.3.9-win-x86.msi

### WSL Installation 2️⃣

wsl --install

### Installing NVM 3️⃣

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash

nvm install --lts

### Rust Installation 4️⃣

sudo apt install build-essential

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

### Setup ICP Environment 5️⃣

sh -ci "$(curl -fsSL https://internetcomputer.org/install.sh)"

*After completing all the steps, we suggest you run the following codes and restart the Ubuntu. 👇

sudo apt-get update -y 

sudo apt install build-essential

sudo apt-get install -y gcc-multilib

rustup self uninstall & curl --proto '=https' --tlsv1.2 https://sh.rustup.rs/ -sSf | sh
