MAZE PROJECT
The Maze is a 3D maze game that uses ray casting to render a 2D map into a 3D navigable world!

The Maze project is written in C using the SDL2 library. The development environment used was Ubuntu 14.04 LTS with gcc (Ubuntu 4.8.4-2ubuntu1~14.04) 4.8.4.

### About SDL2

Simple DirectMedia Layer (SDL) is a cross-platform development library designed to provide low-level access to audio, keyboard, mouse, joystick, and graphics hardware via OpenGL and Direct3D. It is widely used in video playback software, emulators, and popular games including Valve's award-winning catalog and many Humble Bundle games.

## Features

- Real-time 3D rendering using ray casting
- Smooth and responsive controls
- Simple and extensible codebase
- Cross-platform support via SDL2

## Installation

To set up the Maze project on your local machine, follow these steps:

1. Clone the repository:
   ```sh
   $ git clone https://github.com/YOUR_USERNAME/MazeProject.git
   ```

2. Navigate to the project directory:
   ```sh
   $ cd MazeProject
   ```

3. Install SDL2:
   - **Ubuntu/Debian**:
     ```sh
     $ sudo apt-get update
     $ sudo apt-get install libsdl2-dev
     ```
   - **macOS**:
     ```sh
     $ brew install sdl2
     ```
   - **Windows**: Download the development libraries from the [SDL website](https://www.libsdl.org/download-2.0.php) and follow the installation instructions.

## Usage

To run the game, execute the following command in the project directory:

```sh
$ ./maze
```

Alternatively, you can use the `make` command:

```sh
$ make run
```

## Controls

- **Move Forward**: Up Arrow or `W`
- **Move Backward**: Down Arrow or `S`
- **Turn Right**: Right Arrow or `D`
- **Turn Left**: Left Arrow or `A`

## Compilation

To compile the project, use the following command:

```sh
$ gcc -Wall -Werror -Wextra -pedantic ./src/*.c -lm -o maze `sdl2-config --cflags` `sdl2-config --libs`
```

Or simply use the `make` command:

```sh
$ make
```

## Project Structure

```plaintext
MazeProject/
├── headers/
│   ├── maze.h
│   └── renderer.h
├── images/
│   ├── texture1.png
│   └── texture2.png
├── landing_page/
│   ├── index.html
│   └── styles.css
├── src/
│   ├── main.c
│   ├── maze.c
│   └── renderer.c
├── .gitignore
├── AUTHOR
├── Makefile
├── README.md
└── maze
```

- **`headers/`**: Contains header files for the project.
- **`images/`**: Stores texture and image assets.
- **`landing_page/`**: Contains HTML and CSS for the project's landing page.
- **`src/`**: Contains the source files for the project.
- **`.gitignore`**: Specifies files and directories to be ignored by Git.
- **`AUTHOR`**: Contains the author's information.
- **`Makefile`**: Defines rules for building and running the project.
- **`README.md`**: Provides an overview and instructions for the project.
- **`maze`**: The compiled executable (generated after compilation).

## Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgements

- SDL2: [https://www.libsdl.org/](https://www.libsdl.org/)
- Inspiration from various maze and ray casting tutorials available online.

Feel free to contact the project maintainer for any queries or contributions.
```

This `README.md` provides comprehensive information about the project, making it easier for users and contributors to understand and work with the project.
