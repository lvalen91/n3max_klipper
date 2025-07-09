# n3max_klipper
Elegoo Neptune 3 Max - Klipper

As I test Klipper on my Elegoo Neptune 3 Max. I will update these files as I go.

- config is the .config within the klipper directory where you build the firmware, you can copy and paste or select the same options when running menuconfig
  Arch: STM32
  Proc Model: STM32F401  ---- (My Printer Motherboard has teh F402 processor, but its similar enough)
  Clock: 8 Mhz
  Comm - USART2 PA3/PA2  ----- (My J17 UART pins are connected to PA2 and PA3 on the processor. USART1 did not work for me
  Baudrate - 250000

  - Printer.cfg (not uploaded)
    Try out or test any of the printer.cfg online for the Neptune 3 Max
    Verify that serial interface and baud rate are specified.

    I used https://github.com/TheFeralEngineer/Klipper-for-Elegoo-Neptune-series-3D-Printers

[mcu]
baud: 250000

- ZNP_ROBIN_NANO.bin
   This is the firmware I have flashed to the printer. If successful the printer bootloader will rename it with a new extension, .CUR
   I am as of this writing testing my printer with this firmware.
