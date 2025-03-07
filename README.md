# ds3-uw
Dark Souls 3 Ultrawide Patcher

# Dark Souls 3 Ultrawide Patcher (ds3-uw)

This script patches the Dark Souls III executable (`DarkSoulsIII.exe`) to remove black bars when playing on ultrawide monitors. It directly modifies the executable in a temporary directory, leaving your original game files untouched.

## Features

*   Removes black bars for supported ultrawide resolutions.
*   Creates a temporary patched executable; your original `DarkSoulsIII.exe` is not modified.

## Supported Resolutions

The script currently supports the following ultrawide resolutions:

*   2560x1080
*   3440x1440
*   5120x1440

**Adding support for other resolutions requires hex editing and debugging the `DarkSoulsIII.exe` file to determine the correct hex patch for that resolution.**

## Dependencies

*   Python 3 (3.8 or later recommended)

## Installation

1.  **Download:** Download the `ds3-uw` script.
2.  **Place in Game Directory:** Copy the `ds3-uw` script file into your Dark Souls III game directory (the same folder that contains `DarkSoulsIII.exe`). This is typically located at:
    `C:\Program Files (x86)\Steam\steamapps\common\DARK SOULS III\Game\`

## Usage

1.  **Open Steam:** Launch Steam.
2.  **Game Properties:** Right-click on "DARK SOULS III" in your Steam library.
3.  **Properties:** Select "Properties...".
4.  **Launch Options:** In the "General" tab, find the "Launch Options" text box.
5.  **Enter Launch Options:**

    ```
    python ds3-uw 3440x1440 -- %command%
    ```

    ```
    python ds3-uw 2560x1080 -- %command%
    ```

    ```
    python ds3-uw 5120x1440 -- %command%
    ```

7. **Launch:** Launch the game through Steam. The script will automatically create a patched executable and run it.

## Credits
* [Original er-patcher] https://github.com/gurrgur/er-patcher
* [Video with Hex-values] https://www.youtube.com/watch?v=1jP28z9H3Mg
