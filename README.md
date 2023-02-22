# react_ui_template

Boilerplate for prototyping Next.js (TypeScript) applications with Docker.

## Table of Contents

**[Prerequisites](#prerequisites)**  
**[Usage Instructions](#usage-instructions)**  
**[Debugging](#debugging)**

## Prerequisites

### Visual Studio Code

[Download](https://code.visualstudio.com/download) and install Visual Studio Code.

### Docker Desktop

[Download](https://www.docker.com/products/docker-desktop) and install Docker Desktop.

### Node.js

#### Installer

[Download](https://nodejs.org/) Node.js using the installer.

#### Homebrew (macOS)

Install Homebrew:

```console
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Make sure Homebrew is up to date:

```console
brew update
```

Make sure your system is ready:

```console
brew doctor
```

Add Homebrew's location to your `$PATH` in `.bash_profile` or `.zshrc` file.

```console
export PATH="/usr/local/bin:$PATH"
```

Install Node.js:

```console
brew install node
```

## Usage Instructions

1. Download or clone this template repository.
2. Open the project folder with Visual Studio Code.
3. Find and replace all instances of `react_ui_template` with your preferred name.

### Development

Build the image:

```console
docker build -f Dockerfile.dev -t your_image_name:tag .
```

Run a container:

```console
docker run --rm -it -p 3000:3000/tcp -p 9229:9229/tcp your_image_name:tag
```

### Production

Build the image:

```console
docker build -f Dockerfile.prod -t your_image_name:tag .
```

Run a container:

```console
docker run --rm -it -p 3000:3000/tcp your_image_name:tag
```

## Debugging

Debugging is only available for Development. Consider reviewing [this documentation](https://code.visualstudio.com/docs/editor/debugging) if you have not used Visual Studio Code's built-in debugger. Details on how specifically debugging works in Next.js can be found [here](https://nextjs.org/docs/advanced-features/debugging).
