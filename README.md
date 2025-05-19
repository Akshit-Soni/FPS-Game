## FPS Network Shooter Game

A first-person shooter (FPS) built in Unity featuring local network multiplayer using UNet’s low-level networking API. Compete with friends over LAN, enjoy smooth gameplay, and explore basic matchmaking.

---

## Table of Contents

* [Project Overview](#project-overview)
* [Features](#features)
* [Reference Playlist](#reference-playlist)
* [Installation](#installation)
* [Usage](#usage)
* [Networking Architecture](#networking-architecture)
* [Project Structure](#project-structure)
* [Contributing](#contributing)
* [License](#license)

---

## Project Overview

This Unity project demonstrates how to set up a simple local network multiplayer FPS using Unity’s built-in networking (UNet). Players can host or join a game over LAN, control avatars in first-person perspective, and engage in fast-paced shooter matches.

Repository: [https://github.com/Akshit-Soni/FPS-Game](https://github.com/Akshit-Soni/FPS-Game)

## Features

* **Local LAN Multiplayer**: Host or join games within the same network.
* **First-Person Controller**: Smooth player movement, camera look-around, and jumping.
* **Basic Shooting Mechanics**: Raycast-based hits, health management, and respawn.
* **Simple UI**: Host/Join menus, player count, and score display.
* **Matchmaking**: Automatic discovery of hosts on the local network.

## Reference Playlist

This project was built following tutorials in the following YouTube playlist:

[https://youtube.com/playlist?list=PLtLToKUhgzwm1rZnTeWSRAyx9tl8VbGUE](https://youtube.com/playlist?list=PLtLToKUhgzwm1rZnTeWSRAyx9tl8VbGUE)

Special thanks to the creator for clear, step-by-step guidance on UNet and multiplayer setup.

## Installation

1. **Prerequisites**:

   * Unity 2018.4 LTS (or later) installed.
   * Git installed for repository cloning.

2. **Clone the repository**:

   ```bash
   git clone https://github.com/Akshit-Soni/FPS-Game.git
   cd FPS-Game
   ```

3. **Open in Unity**:

   * Launch Unity Hub.
   * Add the `FPS-Game` folder as a project.
   * Open the project in the Unity Editor.

## Usage

* **Host a Game**: In the main menu, click **Host**, then wait for players to join.
* **Join a Game**: Click **Join**, select a host from the discovered list, and connect.
* **Play**: Use `WASD` to move, mouse to look, left-click to shoot, and `Space` to jump.
* **Exit**: Press `Esc` to return to the main menu.

## Networking Architecture

* **Network Manager**: Manages connections, spawning, and matchmaking.
* **Networked Player Prefab**: Contains `NetworkIdentity`, `NetworkTransform`, and custom scripts for movement and shooting.
* **Messaging System**: Uses Commands (`[Command]`) and ClientRpcs (`[ClientRpc]`) for server-authoritative actions and client updates.

## Project Structure

```
FPS-Game/
├── Assets/
│   ├── Scenes/             # Main scene and network lobby scene
│   ├── Scripts/            # PlayerController, GameManager, Network scripts
│   ├── Prefabs/            # Player prefab, UI prefabs
│   └── UI/                 # Canvas, menus, HUD elements
├── ProjectSettings/        # Unity project settings
├── Packages/               # Package manifest
├── .gitignore              # Unity gitignore rules
└── README.md               # This file
```

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m "Add feature"`).
4. Push to your branch (`git push origin feature-name`).
5. Open a Pull Request with a clear description of your changes.

Please follow Unity best practices and document any new scripts or features.

## License

This project is open-source under the MIT License. See [LICENSE](LICENSE) for details.
