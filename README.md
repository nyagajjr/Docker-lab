# Docker Installation and Troubleshooting on macOS

## System Information

- Operating System: macOS
- Architecture: Intel (`x86_64`)
- Shell: Zsh
- Homebrew location: `/usr/local/bin/brew`

## 1. Check Mac Architecture

```bash
uname -m
```

## 2. Check Homebrew Installation

```bash
which brew
brew --version
```

## 3. Configure Homebrew in Zsh

Open the Zsh configuration file:

```bash
nano ~/.zshrc
```

Add or correct the Homebrew initialization line:

```bash
eval "$(/usr/local/bin/brew shellenv)"
```

Save using `Ctrl + O`, press `Enter`, and exit using `Ctrl + X`.

## 4. Reload Zsh Configuration

```bash
source ~/.zshrc
```

## 5. Check Docker Installation

```bash
docker --version
```

Check the Docker executable location:

```bash
which docker
```

## 6. Check Docker Engine

```bash
docker info
```

**Note:** Docker Desktop must be running for the Docker CLI to communicate with the Docker Engine.

## Useful Commands Summary

| Command | Purpose |
|---|---|
| `uname -m` | Check processor architecture |
| `which brew` | Locate Homebrew |
| `brew --version` | Check Homebrew version |
| `source ~/.zshrc` | Reload shell configuration |
| `docker --version` | Check Docker CLI version |
| `which docker` | Locate Docker CLI |
| `docker info` | Inspect Docker Engine |

## Key Concepts

- **Zsh:** The command-line shell used by macOS.
- **.zshrc:** Configuration file for interactive Zsh sessions.
- **PATH:** Environment variable containing directories where executable programs are located.
- **Homebrew:** Package manager for macOS.
- **Docker CLI:** Command-line interface used to interact with Docker.
- **Docker Engine:** Technology responsible for building and running containers.
- **Docker Desktop:** Application that provides Docker Engine and supporting tools on macOS.
