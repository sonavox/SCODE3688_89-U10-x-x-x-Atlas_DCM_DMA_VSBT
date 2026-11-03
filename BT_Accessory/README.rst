BT_Accessory
************

BT accessory firmware for the NXP FRDM-MCXA156 board.

Building
========

Open ``BT_Accessory.code-workspace`` from the repository root, or open the
``BT_Accessory`` application folder in VS Code.

From the application folder::

    cmake --preset debug
    cmake --build --preset debug

The local Zephyr workspace is stored under
``Project_Assets/zephyr_440_mcxa156``. The reusable MCXA library remains
outside this repository under ``../../MCXA_Lib/Lib`` relative to the
repository root.

Firmware outputs are generated in ``BT_Accessory/debug/zephyr``. The UART
firmware tool defaults to ``BT_Accessory/debug/zephyr/zephyr.signed.bin``
when launched from the repository root.
