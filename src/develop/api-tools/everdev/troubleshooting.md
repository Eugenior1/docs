---
title: Troubleshooting
sidebar_position: 2
---

# EverDev Troubleshooting

Here are some solutions to frequently encountered problems.

## EACCESS errors during installation

These errors can occur, if npm was installed without the use of a version manager.

Refer to [this article](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally) for ways to resolve the issue.

## command not found: everdev

This error may happen because `PATH` environment variable was not correctly updated to contain path to Node.js binary.


If you use Linux, ensure the following command is in your `~/.bashrc` for bash shell or `~/.zshrc` for zsh shell:

```sh
export PATH=~/.npm-global/bin:$PATH
```

If you have installed Node.js using Homebrew on MacOS, npm binaries could be found in `/usr/local/share/npm/bin`. 
So, in your `~/.zshrc` file add the following:

```sh
export PATH=/usr/local/share/npm/bin:$PATH
```

If you use Windows, add path to NodeJS bin directory via environment variables settings dialogue and relaunch console window.

Additionally, make sure [permissions are alright](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally).

## Unspecified Error on `everdev sol compile` in Windows 10

1) Run \Users\UserName\everdev\solidity\solc.exe and review error messages.
2) Update Visual Studio components and make sure [vc_redist is installed](https://support.microsoft.com/en-us/topic/the-latest-supported-visual-c-downloads-2647da03-1eea-4433-9aff-95f26a218cc0).

## TON OS SE: Couldn’t connect to Docker daemon

This error occurs in two cases. Either the docker daemon isn't running, or current user doesn't have rights to access docker.

You can [fix the rights](https://docs.docker.com/engine/install/linux-postinstall/) issue either by running relevant commands as the superuser or adding the user to the `docker` group: 

    sudo usermod -a -G docker $USER

Make sure to restart the system or log out and back in, for the new group settings to take effect.

## After everdev is installed on Ubuntu WSL on Windows 10 old version is there

This issue can occur if npm was installed without correct permissions for Linux/Ubuntu.
Refer to [this article](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally) for ways to resolve it.

After it is done, reload terminal and install everdev via `npm i everdev -g' again.

> The documentation in Everscale repository is a community effort. Therefore, everyone can contribute with proposals for new topics, suggest new content elements, participate in editing, and provide ideas that will be of great help for network development. Please be informed that our documentation can be edited via GitHub. It can be found [**here**](https://docs.everscale.network/). 
Please make sure to consult our rules and rewards policy via [**this link**](https://docs.everscale.network/contribute/hot-streams/documentations).  
Also, for any questions that may arise, you can text via this [**Telegram chat**](https://t.me/+C2IpQXWZtCwxYzEy).