
# Tiva C Series EK-TM4C123GXL Bare-Metal Programming

Welcome to the **Tiva C Series EK-TM4C123GXL Bare-Metal Programming** repository! This project showcases how to perform bare-metal programming on the Tiva C Series EK-TM4C123GXL development board. We focus on low-level programming without relying on high-level libraries, providing insights into direct hardware manipulation and microcontroller functionality.

## Project Overview

The Tiva C Series EK-TM4C123GXL board, featuring the TM4C123GH6PM microcontroller, is a powerful platform for embedded system development. This repository provides examples and templates for bare-metal programming, demonstrating how to control peripherals and perform basic operations directly through register manipulation.

### Project Structure

- **Firmware/**: Contains bare-metal code examples and projects for the TM4C123GH6PM microcontroller.
- **Documentation/**: Includes datasheets, reference manuals, and other useful documents.
- **Scripts/**: Provides scripts for setup, building, and flashing the firmware.
- **Images/**: Visual aids for understanding pin configurations and board layout.

## Getting Started

### Prerequisites

Before you start, ensure you have the following:
- **Tiva C Series EK-TM4C123GXL Development Board**
- **ARM Toolchain**: Such as GNU Arm Embedded Toolchain for compiling code.
- **Texas Instruments TivaWare**: For additional drivers and example code.
- **LM Flash Programmer**: For flashing firmware to the TM4C123GH6PM microcontroller.

### Hardware Setup

1. **Connect the Development Board**: Use a micro-USB cable to connect the EK-TM4C123GXL to your computer.
2. **Power the Board**: Ensure the board is powered on.

### Software Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/TIVA-C-EK-TM4C123GXL-BSP.git
   cd TIVA-C-EK-TM4C123GXL-BSP
   ```

2. **Install the ARM Toolchain:**

   Follow the instructions from the [ARM Developer website](https://developer.arm.com/tools-and-software/embedded/arm-development-tools/gnu-toolchain/gnu-rm) to install the GNU Arm Embedded Toolchain.

3. **Install TivaWare:**

   Download and install TivaWare from the [Texas Instruments website](https://www.ti.com/tool/SW-TM4C).

4. **Build the Firmware:**

   Navigate to the `Firmware/` directory and use the provided Makefile to build the project:

   ```bash
   cd Firmware
   make
   ```

5. **Flash the Firmware:**

   Use the LM Flash Programmer to upload the compiled firmware (`.bin` or `.hex` file) to the TM4C123GH6PM microcontroller.

   - Open LM Flash Programmer.
   - Select the appropriate COM port and connect to the board.
   - Load the firmware file and program the microcontroller.

## Examples

Here are some example projects included in this repository:

- **01-Blinky**: A simple LED blinking example demonstrating basic GPIO control.
- **02-Button-LED**: An example showing how to toggle an LED based on a button press.
- **03-UART**: A basic UART communication example for sending and receiving data over serial.

Each example includes a README file with detailed instructions on building, flashing, and running the code.

## Documentation

- **Datasheet**: [TM4C123GH6PM Datasheet](https://www.ti.com/lit/ds/symlink/tm4c123gh6pm.pdf)
- **Reference Manual**: [TM4C123GH6PM Reference Manual](https://www.ti.com/lit/ug/spmub4b/spmub4b.pdf)
- **TivaWare Documentation**: Available in the TivaWare installation directory.

## Troubleshooting

- **LED Not Blinking**: Check the GPIO pin configuration and ensure the LED is correctly connected to the designated pin.
- **Build Errors**: Verify that the ARM toolchain and TivaWare are properly installed and configured.

## Contributing

Contributions are welcome! If you have improvements or new examples to add, please fork the repository, make your changes, and submit a pull request. Ensure that your code adheres to the project's coding standards and includes appropriate documentation.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

