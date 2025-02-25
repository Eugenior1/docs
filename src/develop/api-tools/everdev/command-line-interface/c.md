---
title: C++ Compiler
sidebar_position: 0
---

# C++

## Create your first contract

This command creates a basic C++ contract with comments that you can observe and compile.

```shell
everdev clang create Contract
```

## Compile

This command compiles and links a selected C++ contract. After successful compilation you get .abi.json and .tvc files that you can later [use in your DApps to deploy and run contract methods](https://docs.everos.dev/ever-sdk/guides/work_with_contracts/add_contract_to_your_app).

```shell
everdev clang compile Contract.cpp
```

## Version

This command shows the currently installed C++ compiler version.

```shell
everdev clang version
```

## Update

This command updates the compiler to the latest version.

```shell
everdev clang update
```

Use `--force` or `-f` option to force reinstall, if the compiler is already up to date.

## Set

This command sets the compiler version and downloads it if needed.

```shell
everdev clang set --compiler 7.0.0
```

Use `--force` or `-f` option to force reinstall, if the current version is the same as the requested version.

> The documentation in Everscale repository is a community effort. Therefore, everyone can contribute with proposals for new topics, suggest new content elements, participate in editing, and provide ideas that will be of great help for network development. Please be informed that our documentation can be edited via GitHub. It can be found [**here**](https://docs.everscale.network/). 
Please make sure to consult our rules and rewards policy via [**this link**](https://docs.everscale.network/contribute/hot-streams/documentations).  
Also, for any questions that may arise, you can text via this [**Telegram chat**](https://t.me/+C2IpQXWZtCwxYzEy).