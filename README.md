# Running project as dev container
## Installation 

To get started, follow these steps:

1. Install and configure Docker for your operating system.
	### Windows / macOS:
	1. Install [Docker Desktop for Windows/Mac](https://www.docker.com/products/docker-desktop).
	2. If you are using WSL 2 on Windows, to ensure the [WSL 2 back-end](https://aka.ms/vscode-remote/containers/docker-wsl2) is enabled: Right-click on the Docker taskbar item and select Settings. Check Use the WSL 2 based engine and verify your distribution is enabled under Resources > WSL Integration.
	3. When not using the WSL 2 back-end, right-click on the Docker task bar item, select Settings and update Resources > File Sharing with any locations your source code is kept. See [tips and tricks](https://code.visualstudio.com/docs/remote/troubleshooting#_container-tips) for troubleshooting.

	### Linux:
	1. Follow the official install instructions for Docker CE/EE for your distribution. If you are using Docker Compose, follow the Docker Compose directions as well.

	2. Add your user to the docker group by using a terminal to run: sudo usermod -aG docker $USER

	3. Sign out and back in again so your changes take effect.
 
2. Install [Visual Studio Code](https://code.visualstudio.com/) or [Visual Studio Code Insiders](https://code.visualstudio.com/insiders/).

3. Install the [Remote Development extension pack](https://aka.ms/vscode-remote/download/extension).

## Running the container project

1. Open folder containing the project in VSCode

2. Type command/shift/p to bring up the command pallette

3. Type "Remote Containers: Reopen in container" and hit enter

4. Type "Remote Containers: Rebuild container" and hit enter again

4. Wait for the container to build and start, this may take a while the first time. Once the 
build is complete, type F5 to start debugging the project.

## Source Control
The container project uses git for source control. If you use git SSH keys, make sure to set ForwardAgent yes for any key you want to share with the container.

## Running Project locally
1. Run ```npm i``` to install dependencies
2. Run ```npm run dev``` to start the project

