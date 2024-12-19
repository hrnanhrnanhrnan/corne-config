# Corne Keyboard Configuration (ZMK)

This repository contains my personal configuration for the **Corne mechanical keyboard**, using [ZMK Firmware](https://zmk.dev/). It is set up to automatically build the firmware via GitHub Actions, making it easy to download and flash onto your keyboard.

## Features

- **ZMK Configurations**: Fully customizable keymap and features.
- **GitHub Actions**: Automatically builds the firmware when you push changes to the repository.
- **Custom Layers**: Includes layers for navigation, media, and additional shortcuts.
- **Downloadable Firmware**: Pre-built firmware is available for direct download under the Actions section, and the latest build.

## Getting Started

### Using the Pre-Built Firmware

1. Navigate to the [Releases](https://github.com/hrnanhrnanhrnan/corne-config/actions) section of this repository.
2. Download the latest firmware file from the artifacts of the latest build and unpack to see a `.uf2` file for each half of your Corne keyboard.
3. Flash the downloaded files onto each half of your keyboard using your preferred method.

### Customizing Your Configuration

If you'd like to customize the configuration:
1. Fork this repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/corne-config.git
   ```
2. Make adjustments to the configuration files in the repository. You can refer to the [ZMK documentation](https://zmk.dev/docs) for guidance.
3. Push your changes to your forked repository. The GitHub Actions workflow will automatically build your firmware.
4. Download the firmware artifact from the Actions tab in your forked repository:
   - Go to **Actions** -> Select the latest workflow run -> Download the firmware from the artifacts section.

## Repository Structure

- `config/`: Contains the main configuration files for ZMK.
- `keymaps/`: Includes the keymap definitions for your Corne keyboard.
- `.github/workflows/`: Contains the GitHub Actions workflow file for building the firmware.
- `readme.md`: This document.

## How It Works

1. On every push to this repository, a GitHub Action triggers the build process.
2. The firmware is compiled using the configuration files in the repository.
3. The compiled `.uf2` files is available as an artifact zipped as a firmware file in the latest action build, see [Action](https://github.com/hrnanhrnanhrnan/corne-config/actions) section.

## Contributions

Feel free to fork this repository and customize it to your liking. If you have suggestions or improvements, consider opening an issue or pull request.

## Acknowledgments

- Thanks to the [ZMK Firmware](https://zmk.dev/) community for providing a robust framework for keyboard firmware.
- Credit to the creators of the Corne keyboard for an amazing ergonomic split design.
- Easy edits is also possible through the amazing website [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/). Just connect to your github repository and get a GUI version of the keyboard to make customization extremely easy. Commit and push directly from the website by just clicking save. 