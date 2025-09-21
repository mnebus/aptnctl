# aptnctl

A simple CLI wrapper for managing a local MicroK8s Kubernetes cluster. Simplifies starting, stopping, and querying your cluster with commands like `aptnctl start`, `aptnctl stop`, `aptnctl get pods`, and `aptnctl logs <pod>`.

## Installation

### Prerequisites
- Install MicroK8s: `snap install microk8s --classic`
- Homebrew (for macOS/Linux)

### Via Homebrew
1. Tap the repository:
   ```bash
   brew tap mnebus/homebrew-aptnctl
   ```
2. Install aptnctl:
   ```bash
   brew install aptnctl
   ```

### Manual Installation
1. Clone the repo:
   ```bash
   git clone https://github.com/mnebus/aptnctl.git
   ```
2. Copy the script to your PATH:
   ```bash
   chmod +x aptnctl
   sudo mv aptnctl /usr/local/bin/
   ```

## Usage
- Start the cluster with DNS and Ingress: `aptnctl start`
- Stop the cluster: `aptnctl stop`
- Get resources: `aptnctl get pods`
- View logs: `aptnctl logs <pod-name>`

## Notes
- Assumes MicroK8s is installed and configured.
- Use `nip.io` for local subdomain routing (e.g., `http://service1.127.0.0.1.nip.io`).
- Licensed under MIT. Contributions welcome!