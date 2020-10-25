VS Code setup for nRF52 BLE template
===

The nRF52 SDK BLE template project setup for use with Visual Studio Code and the gcc toolchain.

Prerequisites
-

Install the [Nordic nRF5 SDK](https://www.nordicsemi.com/Software-and-tools/Software/nRF5-SDK) and the [gcc ARM toolchain](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads). For the latter, on OS X you can conveniently install the gcc tooling view homebrew via `brew install arm-none-eabi-gcc` you may need to `brew tap ArmMbed/homebrew-formulae` if you haven't already done so.

Editing
===

The following environment variables require declaration:

```
export SDK_ROOT=<path to the nRF sdk e.g. /opt/nordic/nRF5_SDK_17.0.2_d674dde>
export GNU_INSTALL_ROOT=<path to the gcc toolchain binaries e.g. /usr/local/bin/>
```

For MacOS, you can then open this work space and inherit the environment vars:

```
open vs_ble_app_template.code-workspace
```

Building
===

> Note that you will need to configure the nRF5 SDK to reflect the location of the build tools. For example, on Unix, edit to the `components/toolchain/gcc/Makefile.posix` file.

Various build tasks have been configured. Please check out the tasks menu.
