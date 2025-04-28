# Zen Browser XBPS Package

This repository contains files for packaging Zen Browser for Void Linux using the XBPS package manager.

## Files

1. `template`: XBPS template file for Zen Browser

## Template File

The `template` file is an XBPS template for Zen Browser.

- Architecture: x86_64 only
- Build style: precompiled binaries

The template file handles the installation of precompiled binaries and sets up the necessary dependencies.

### Installation

To install the Zen Browser package:

1. Clone the Void Packages repository:
   ```sh
   git clone https://github.com/ihateemoji/zen-browser.git
   ```
2. Copy the directory to the `srcpkgs/zen-browser` directory in your Void Packages repository:
   ```sh
   cp -rf zen-browser /path/to/void-packages/srcpkgs/
   ```
3. Build the package:
   ```sh
   ./xbps-src pkg zen-browser
   ```
4. Install the package:
   ```sh
   sudo xbps-install --repository=hostdir/binpkgs zen-browser
   ```
5. Run Zen Browser:
   ```sh
   zen
   ```
6. Enjoy!

* You can also install using `vpsm` instead of (3) and (4):
   ```sh
   vpsm install zen-browser
   ```

## Contributing

If you want to contribute to this package, please make sure to test your changes thoroughly before submitting a pull request.

## Issues

If you encounter any issues with the package or the update script, please open an issue in this repository.
