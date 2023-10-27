# Ball Picking Project

This repository acts as the main repository to be deployed on the Agile-X Scout2.0 robot for the AUS/IFRoS lab 2023 project of searching for and picking up tennis balls.

## Setup

### 1. Clone this repository recursively on the Scout2.0

```bash
git clone --recurse-submodules https://github.com/IFRoS-ELTE/ball_picking_project.git
```

### 2. Build and launch the containers

```bash
cd ./ball_picking_project && sudo docker compose up
```

### Stopping and re-launching

To stop and close the nodes, simply use `CTRL+C`, this will stop all containers. You can use `sudo docker compose up` if you want to re-launch. If you, for some reason, want to remove the containers, you can do so with the `sudo docker compose down` command. This means that at the next startup using `sudo docker compose up`, the containers will be newly created and all the ros workspaces inside will have to be freshly built as well.
