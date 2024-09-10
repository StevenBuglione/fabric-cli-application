# Fabric CLI Action Demo

This repository demonstrates how an external repository can reference and use the `StevenBuglione/fabric-cli-action@v1.0` GitHub Action. This action is designed to interact with the Microsoft Fabric API.

## Workflow

The main workflow of this repository is defined in the `.github/workflows/main-fabric.yml` file. This workflow is triggered on every push to the `main` branch.

The workflow consists of two jobs:

1. `create-workspaces`: This job uses the `StevenBuglione/fabric-cli-action@v1.0` action to create a new workspace. The ID of the GitHub run is used as the value for the workspace.

2. `list-workspaces`: This job lists all the workspaces. It depends on the `create-workspaces` job and also uses the `StevenBuglione/fabric-cli-action@v1.0` action.

## Usage

To use this repository as a reference, you can view the `main-fabric.yml` file to understand how to use the `StevenBuglione/fabric-cli-action@v1.0` action in your own workflows.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.         