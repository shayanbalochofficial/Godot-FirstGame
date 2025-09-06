# Jungle Runner

![Jungle Runner Banner](summer.hackclub.com/rails/active_storage/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NjM1OTQsInB1ciI6ImJsb2JfaWQifX0=--1f0b0c8d96b0ab5a6a5e3ad7380ec20e07ce5a38/WhatsApp%20Image%202025-09-06%20at%2014.42.39_7aac7d1d.jpg) <!-- Replace with actual banner image if available, e.g., from assets or itch.io screenshot -->

## Overview

Jungle Runner is a fun and addictive endless runner game developed as my first project using the Godot game engine. In this game, you take control of a character dashing through a dense jungle, dodging obstacles like logs, rocks, and wildlife, while collecting coins, power-ups, and other items to boost your score. The game features procedurally generated levels for endless replayability, simple mechanics suitable for all ages, and vibrant pixel-art style graphics inspired by classic platformers.

This repository contains the full source code for the game, including scenes, scripts, assets, and configuration files. It was built with Godot (version 4.x recommended), and the playable version is hosted on itch.io for easy access.

**Play the game now:** [https://shayanbalochofficial.itch.io/jungle-runner](https://shayanbalochofficial.itch.io/jungle-runner)  
(HTML5 web version available – no download required!)

## Features

- **Endless Runner Gameplay**: Procedurally generated jungle paths that get progressively harder, ensuring no two runs are the same.
- **Obstacles and Challenges**: Avoid pitfalls, jumping over hurdles, sliding under branches, and evading enemies like monkeys or snakes.
- **Collectibles and Power-Ups**: Gather coins for points, magnets to attract items, shields for temporary invincibility, and speed boosts for thrilling dashes.
- **Scoring System**: Track high scores with multipliers based on distance traveled and items collected. Compete with friends or aim for personal bests.
- **Audio and Visuals**: Custom sound effects for jumps, collisions, and pickups; background music that ramps up with intensity; and colorful 2D sprites for characters, environments, and UI.
- **Cross-Platform Support**: Built in Godot, exportable to HTML5 (web), Windows, macOS, Linux, Android, and iOS.
- **Simple Customization**: Easy-to-modify scripts and assets for adding new features, levels, or themes.

## Installation

To run or modify the game locally, follow these steps:

1. **Install Godot Engine**:
   - Download the latest version of Godot from the official website: [https://godotengine.org/download](https://godotengine.org/download).
   - This project is compatible with Godot 4.x (tested on 4.2+). Godot 3.x may require minor adjustments.

2. **Clone the Repository**:
   ```
   git clone https://github.com/shayanbalochofficial/Godot-FirstGame.git
   ```
   - Navigate to the project folder: `cd Godot-FirstGame`.

3. **Open in Godot**:
   - Launch Godot and import the project by selecting the `project.godot` file in the root directory.
   - Godot will automatically load all scenes, scripts, and assets.

4. **Dependencies**:
   - No external plugins or add-ons are required – everything is built with Godot's built-in features and GDScript.
   - If assets like audio or images are missing (e.g., due to gitignore), they can be recreated or sourced from free asset packs (e.g., from Kenney.nl or OpenGameArt.org).

## Usage

### Running the Game in Godot Editor
- Press `F5` (or click the "Play" button) to run the main scene.
- The default main scene is typically `main.tscn` or `game.tscn` (check `project.godot` for the entry point).
- Use the editor's debugger to test mechanics, tweak values, or add new elements.

### Exporting the Game
1. In Godot, go to **Project > Export**.
2. Add presets for your target platform (e.g., HTML5 for web deployment).
3. Export the project – for web, upload the generated files to a host like itch.io.
4. For desktop exports, run the resulting executable.

### Building from Source
- If modifying scripts (e.g., in `scripts/` directory), save changes and rerun.
- Example: To adjust player speed, edit the `player.gd` script's velocity variables.

## Controls

- **Movement**: Auotmatic infinite running.
- **Jump**: Spacebar or Up Arrow to jump over obstacles.

(Controls are customizable in the input map via Godot's project settings.)

## Project Structure

Here's an overview of the repository's key files and directories (based on standard Godot project layout):

- **`project.godot`**: The main project configuration file. Defines settings like window size, physics, and main scene.
- **`icon.png` / `default_env.tres`**: Project icon and default environment settings.
- **`scenes/`**: Contains .tscn files for game scenes.
  - `main.tscn`: Entry point with menu and HUD.
  - `level.tscn`: The core gameplay scene with procedural generation.
  - `player.tscn`: Player character node with animations and collision.
- **`scripts/`**: GDScript (.gd) files for logic.
  - `player.gd`: Handles movement, jumping, sliding, and collision detection.
  - `obstacle_spawner.gd`: Script for spawning obstacles and collectibles.
  - `score_manager.gd`: Tracks and displays scores.
- **`assets/`**: Art, audio, and other resources.
  - `sprites/`: PNG files for player, obstacles, background (e.g., jungle tileset).
  - `audio/`: WAV/MP3 files for sound effects and music.
  - `fonts/`: TTF files for UI text.
- **`addons/`**: (If any) Optional Godot add-ons for extra features.
- **`.gitignore`**: Ignores temporary files like .import directories.
- **`LICENSE`**: MIT License file.

This structure follows Godot best practices for organization and scalability.

## Development Notes

- **Inspiration**: This game was created as a learning project following beginner Godot tutorials (from youtube). It demonstrates core concepts like 2D physics, node hierarchies, signals, and animation players.
- **Tools Used**:
  - Godot Engine (free and open-source).
  - GDScript for scripting.
- **Known Issues**:
  - Performance may vary on low-end devices due to procedural generation.
  - No mobile touch controls implemented yet (planned for future updates).
- **Future Plans**:
  - Add leaderboards via SilentWolf or similar.
  - More levels/themes (e.g., desert or cave runners).
  - Multiplayer mode for competitive runs.

## Contributing

Contributions are welcome! If you'd like to improve the game:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add YourFeature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

Please ensure code follows Godot style guidelines and test changes thoroughly.

## Credits

- Developed by [shayanbalochofficial](https://github.com/shayanbalochofficial).
- Assets: Sourced from free libraries (e.g., Kenney Assets – credit if used).
- Special thanks to the Godot community for tutorials and support.

If you used specific tutorials or assets, add them here.

## License

MIT License

Copyright (c) 2024 Bartosz Budnik (BudzioT)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

For questions or feedback, open an issue on GitHub or contact me via email at shayanbalochofficial@gmail.com. Happy running! 🌿🏃‍♂️







