# AppRunner Demo

Example app demonstrating AWS AppRunner deployment both from source code as well
as container image. This was presented in a meetup of AWS User Group Montenegro.

## Prerequisites

To follow this guide you need:

- an AWS account
- [AWS Copilot CLI](https://aws.github.io/copilot-cli/docs/getting-started/install/)
- [Docker](https://docs.docker.com/engine/install/)

## Getting Started

We'll use AWS console for deploying the app using GitHub integration. To deploy
the app using AWS copilot CLI follow the steps bellow:

1. initialize the app
```shell
copilot app init
```
2. initialize the environments
```shell
copilot env init --name dev
copilot env init --name prod
```
3. deploy the environments
```shell
copilot env deploy --name dev
copilot env deploy --name prod
```
4. deploy the service
```shell
copilot deploy --name dev
copilot deploy --name prod
```

## Cleanup

To clean up resources created during the demo run:

```shell
copilot app delete
```
