# ThreeMod

ThreeMod is an AI-native game engine for creating games and interactive content without writing code. Create projects in the desktop app, export them as bundles, and play them in a web browser.

[Desktop downloads](https://github.com/Niceofer/ThreeMod/releases) · [Website](https://threemod.com) · [Discord](https://discord.gg/aFjbNBh6)

[한국어](./README_ko.md) · [日本語](./README_ja.md)

## Download and install

Download and install the package for your operating system from [GitHub Releases](https://github.com/Niceofer/ThreeMod/releases).

- **Windows**: Run the Windows installer. See also the [Windows installation guide](./INSTALL_BYC_WINDOWS.md).
- **macOS**: Download the macOS package and install the app. Requires macOS 13 Ventura or later.

The desktop app is currently unsigned, so your operating system may display a security warning. On Windows, check **More info → Run anyway**. On macOS, use **right-click → Open** in Finder or check the option to allow the app in **System Settings → Privacy & Security**.

## Create and play projects

Create and edit projects in the ThreeMod desktop app. In the project details panel, select **Export bundle → Export to folder** to export the project data and required assets.

Run exported bundles with the [`source` player](./source/README.md) in this repository. Place bundles in `source/share_data`, start the player, and open **http://localhost:3300** to play from the project home screen. See the [player README](./source/README.md) for installation and startup commands.

![Project bundle deployment workflow](./author-export-play.svg)

## Browser examples

Try content created with ThreeMod directly in your browser, without installing anything.

- [Life Simulation](https://share.threemod.com/byc_f8b97ef4c16045149399d27014556e48)
- [Interaction](https://share.threemod.com/byc_b0cc670cf88f4838b6e1abd80e7755d5)

## Repository layout

- **Root**: Introduction, installation instructions, and related materials for the ThreeMod desktop packages available in Releases
- **[`source/`](./source/)**: Player source and instructions for running project bundles in a local web browser

## Publish your project

To make your project available to others, upload the player and bundles to a cloud server and serve them through a domain or static IP address.

## Terms of use

[License](./LICENSE.md) · [EULA](./EULA.md) · [Third-party notices](./THIRD-PARTY-LICENSES.md)
