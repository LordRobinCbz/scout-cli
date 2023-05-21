_Note:_ Docker Scout is a new product and is free while in early access. Read more about [Docker Scout](https://www.docker.com/products/docker-scout?utm_source=hub&utm_content=scout-action-readme).

- [Docker Scout](#docker-scout)
- [Usage](#usage)
- [CLI Plugin Installation](#cli-plugin-installation)
 
# Docker Scout

[Docker Scout](https://www.docker.com/products/docker-scout/) is a collection of software supply chain features that appear throughout Docker user interfaces and the command line interface (CLI). These features provide detailed insights into the composition and security of container images.

This repository contains the source code of the `docker scout` CLI plugin.

## Usage

See the [reference documentation](https://docs.docker.com/scout) to learn about Docker Scout including Docker Desktop and Docker Hub integrations.

## CLI Plugin Installation

### Docker Desktop

`docker scout` CLI plugin is available by default on [Docker Desktop](https://docs.docker.com/desktop/) starting with version `4.17`.

### Manual Installation

To install it manually:

- Download the `docker-scout` binary corresponding to your platform from the [latest](https://github.com/docker/scout/releases/latest) or [other](https://github.com/docker/scout/releases) releases.
- Uncompress it as
    - `docker-scout` on _Linux_ and _macOS_
    - `docker-scout.exe` on _Windows_
- Copy it in your local CLI plugin directory
    - `$HOME/.docker/cli-plugins` on _Linux_ and _macOS_
    - `%USERPROFILE%\.docker\cli-plugins` on _Windows_
- Make it executable on _Linux_ and _macOS_
    - `chmod +x $HOME/.docker/cli-plugins/docker-scout`
- Authorize the binary to be executable on _macOS_
    - `xattr -d com.apple.quarantine $HOME/.docker/cli-plugins/docker-scout`
