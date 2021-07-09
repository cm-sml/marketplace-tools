# Overview

This repository contains the `mpdev` tool supporting the development of VMs deployable via
[Google Cloud Marketplace](https://console.cloud.google.com/marketplace).

# Installation

## Prerequisites

The following tools must be installed before using `mpdev`.
* [docker](https://docs.docker.com/get-docker/)
* [gsutil](https://cloud.google.com/storage/docs/gsutil_install)
* zip `sudo apt-get install zip`

## Options

### Download latest release

https://github.com/GoogleCloudPlatform/marketplace-tools/releases/latest

### Install with Homebrew

```
brew tap GoogleCloudPlatform/marketplace-tools https://github.com/GoogleCloudPlatform/marketplace-tools.git
```

Output 
```
brew tap GoogleCloudPlatform/marketplace-tools https://github.com/GoogleCloudPlatform/marketplace
-tools.git
==> Tapping googlecloudplatform/marketplace-tools
Cloning into '/usr/local/Homebrew/Library/Taps/googlecloudplatform/homebrew-marketplace-tools'...
remote: Enumerating objects: 754, done.
remote: Counting objects: 100% (228/228), done.
remote: Compressing objects: 100% (169/169), done.
remote: Total 754 (delta 91), reused 119 (delta 37), pack-reused 526
Receiving objects: 100% (754/754), 20.47 MiB | 1.54 MiB/s, done.
Resolving deltas: 100% (349/349), done.
Tapped 1 formula (62 files, 20.8MB).
```
Install mpdev in the downloaded directory 
> cd /usr/local/Homebrew/Library/Taps/googlecloudplatform/homebrew-marketplace-tools

```
brew install mpdev
```
Output 
```
homebrew-marketplace-tools % brew install mpdev
==> Installing mpdev from googlecloudplatform/marketplace-tools
==> Downloading https://github.com/GoogleCloudPlatform/marketplace-tools/releases/download/v0.1.1/mpdev_darwin_amd64_v0.1.1
==> Downloading from https://github-releases.githubusercontent.com/267374160/3a7c7900-973c-11eb-8766-7f7c9ccb0efd?X-Amz-Alg
######################################################################## 100.0%
🍺  /usr/local/Cellar/mpdev/0.1.1: 5 files, 49MB, built in 11 seconds
```



### Build from source

Building from source requires the following:
* [bazel](https://docs.bazel.build/versions/master/install.html)
* [golang](https://golang.org/dl/)

```
make build
```

The mpdev binary will be created at `bazel-bin/mpdev/mpdev_/mpdev`

## Getting Started

See the [mdpev reference](./docs/mpdev-reference.md) 
and [Deployment Manager guide](./docs/deployment-manager-guide.md) documentation.
