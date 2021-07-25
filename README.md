# awesome-zephyr

The Zephyr RTOS ([Zephyr Project](https://www.zephyrproject.org/)) is awesome!

[<img src="https://raw.githubusercontent.com/fkromer/awesome-zephyr/master/logo.svg?sanitize=true" align="right" width="86">](https://www.zephyrproject.org/)

## Contents

- [Zephyr core components](#zephyr-core-components)
- [Guides](#guides)
- [Best Practices](#best-practices)
- [Suggested uses](#suggested-uses)
- [API reference](#api-reference)
- [Zephyr modules](#zephyr-modules)
- [Virtualization](#virtualization)
- [Hardware Abstraction](#hardware-abstraction)
- [Releases](#releases)
- [VSCode extensions](#vscode-extensions)
- [Development containers](#development-containers)
- [Development frameworks](#development-frameworks)
- [Blog posts](#blog-posts)
- [Videos](#videos)

## Zephyr core components

- [Zephyr](https://github.com/zephyrproject-rtos/zephyr) - Zephyr RTOS.
- [west](https://github.com/zephyrproject-rtos/west) - Meta tool.
- [cmake](https://cmake.org/) - Build system.
- [Make](https://www.gnu.org/software/make/) - Build tool (option 1).
- [Ninja](https://ninja-build.org/) - Build tool (option 2).
- [Kconfig](https://www.kernel.org/doc/html/latest/kbuild/kconfig-language.html) - Build configuration.
- [devicetree](https://www.devicetree.org/) - Hardware description.

## Guides

Zephyr v2.6.99

- [Getting Started Guide](https://docs.zephyrproject.org/latest/getting_started/index.html)
- [Beyond the Getting Started Guide](https://docs.zephyrproject.org/latest/guides/beyond-GSG.html)
- [User and Developer Guides](https://docs.zephyrproject.org/latest/guides/index.html)
- [Secure Coding](https://docs.zephyrproject.org/latest/security/secure-coding.html)
- [Board Porting Guide](https://docs.zephyrproject.org/latest/guides/porting/board_porting.html)
- [Devicetree Guide](https://docs.zephyrproject.org/latest/guides/dts/index.html)
- [Architecture Porting Guide](https://docs.zephyrproject.org/latest/guides/porting/arch.html)
- [Architecture-related Guides](https://docs.zephyrproject.org/latest/guides/arch/index.html)
- [Contribution Guidelines](https://docs.zephyrproject.org/latest/contribute/index.html)

## Best Practices

Zephyr v2.6.99

- [Kconfig - Tips and Best Practices](https://docs.zephyrproject.org/latest/guides/build/kconfig/tips.html)

## Suggested uses

Zephyr v2.6.99

- Kernel Services
  - Scheduling, Interrupts, and Synchronization
    - [Threads](https://docs.zephyrproject.org/latest/reference/kernel/threads/index.html#suggested-uses)
    - [Scheduling](https://docs.zephyrproject.org/latest/reference/kernel/scheduling/index.html#suggested-uses)
    - [System Threads](https://docs.zephyrproject.org/latest/reference/kernel/threads/system_threads.html#suggested-uses)
    - [Workqueue Threads](https://docs.zephyrproject.org/latest/reference/kernel/threads/workqueue.html#suggested-uses)
    - [Zephyr Without Threads](https://docs.zephyrproject.org/latest/reference/kernel/threads/nothread.html)
    - [Interrupts](https://docs.zephyrproject.org/latest/reference/kernel/other/interrupts.html#suggested-uses)
    - [Polling API](https://docs.zephyrproject.org/latest/reference/kernel/other/polling.html#suggested-uses)
    - [Semaphores](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/semaphores.html#suggested-uses)
    - [Mutexes](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/mutexes.html#suggested-uses)
    - [Condition Variables](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/condvar.html#suggested-uses)
    - [Symmetric Multiprocesssing](https://docs.zephyrproject.org/latest/reference/kernel/smp/smp.html)
  - Data Passing
    - [FIFOs](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/fifos.html#suggested-uses)
    - [LIFOs](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/lifos.html#suggested-uses)
    - [Stacks](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/stacks.html#suggested-uses)
    - [Message Queue](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/message_queues.html#suggested-uses)
    - [Mailboxes](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/mailboxes.html#suggested-uses)
    - [Pipes](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/pipes.html#suggested-uses)
  - Memory Management
    - [Memory Heaps](https://docs.zephyrproject.org/latest/reference/kernel/memory/heap.html#suggested-uses)
    - [Memory Slabs](https://docs.zephyrproject.org/latest/reference/kernel/memory/slabs.html#suggested-uses)
  - Timing
    - [Timers](https://docs.zephyrproject.org/latest/reference/kernel/timing/timers.html#suggested-uses)
  - Other
    - [CPU Idling](https://docs.zephyrproject.org/latest/reference/kernel/other/cpu_idle.html?highlight=suggested%20uses#suggested-uses)
    - [Atomic services](https://docs.zephyrproject.org/latest/reference/kernel/other/atomic.html?highlight=suggested%20uses#suggested-uses)
    - [Floating Point Services](https://docs.zephyrproject.org/latest/reference/kernel/other/float.html#suggested-uses)
    - [C++ Support for Applications](https://docs.zephyrproject.org/latest/reference/kernel/other/cxx_support.html)

## API reference

Zephyr v2.6.99

- [API Status](https://docs.zephyrproject.org/latest/reference/api/index.html)

- Audio
  - [codec](https://docs.zephyrproject.org/latest/reference/audio/codec.html) - The Audio Codec API provides access to digital audio codecs.
  - [dmic](https://docs.zephyrproject.org/latest/reference/audio/dmic.html) - The audio DMIC interface provides access to digital microphones.
  - [i2s](https://docs.zephyrproject.org/latest/reference/audio/i2s.html) - The I2S (Inter-IC Sound) API provides support for the standard I2S interface as well as common non-standard extensions such as PCM Short/Long Frame Sync and Left/Right Justified Data Formats.
- [Asynchronous Notification](https://docs.zephyrproject.org/latest/reference/misc/notify.html)
- [Bluetooth](https://docs.zephyrproject.org/latest/reference/bluetooth/index.html)
- [Crypto](https://docs.zephyrproject.org/latest/reference/crypto/index.html#) - Crypto (hardware) related functionalities.
- [Devicetree](https://docs.zephyrproject.org/latest/reference/devicetree/index.html)
- [Device Driver Model](https://docs.zephyrproject.org/latest/reference/drivers/index.html)
- [Display Interface](https://docs.zephyrproject.org/latest/reference/display/index.html)
- [Error Detection And Correction (EDAC)](https://docs.zephyrproject.org/latest/reference/edac/index.html)
- [File Systems](https://docs.zephyrproject.org/latest/reference/file_system/index.html)
- [Formatted Output](https://docs.zephyrproject.org/latest/reference/misc/formatted_output.html)
- Kernel Services
  - Scheduling, Interrupts, and Synchronization
    - [Threads](https://docs.zephyrproject.org/latest/reference/kernel/threads/index.html#api-reference)
    - [Workqueue Threads](https://docs.zephyrproject.org/latest/reference/kernel/threads/workqueue.html#api-reference)
    - [Interrupts](https://docs.zephyrproject.org/latest/reference/kernel/other/interrupts.html#api-reference)
    - [Polling](https://docs.zephyrproject.org/latest/reference/kernel/other/polling.html#api-reference)
    - [Semaphores](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/semaphores.html#api-reference)
    - [User Mode Semaphores](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/semaphores.html#user-mode-semaphore-api-reference)
    - [Mutexes](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/mutexes.html#api-reference)
    - [Futex Mutexes](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/mutexes.html#futex-api-reference)
    - [User Mode Mutexes](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/mutexes.html#user-mode-mutex-api-reference)
    - [Condition Variables](https://docs.zephyrproject.org/latest/reference/kernel/synchronization/condvar.html#api-reference)
  - Data Passing
    - [Queues](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/queues.html#api-reference)
    - [FIFOs](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/fifos.html#api-reference)
    - [LIFOs](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/lifos.html#api-reference)
    - [Stacks](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/stacks.html#api-reference)
    - [Message Queues](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/message_queues.html#api-reference)
    - [Mailboxes](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/mailboxes.html#api-reference)
    - [Pipes](https://docs.zephyrproject.org/latest/reference/kernel/data_passing/pipes.html#api-reference)
  - Memory Management
    - [Memory Heap](https://docs.zephyrproject.org/latest/reference/kernel/memory/heap.html#api-reference)
    - [Memory Slabs](https://docs.zephyrproject.org/latest/reference/kernel/memory/slabs.html#api-reference)
  - Timing
    - [Kernel Timing](https://docs.zephyrproject.org/latest/reference/kernel/timing/clocks.html#api-reference)
    - [Timers](https://docs.zephyrproject.org/latest/reference/kernel/timing/timers.html#api-reference)
  - Other
    - [CPU Idling](https://docs.zephyrproject.org/latest/reference/kernel/other/cpu_idle.html#api-reference)
    - [Atomic Services](https://docs.zephyrproject.org/latest/reference/kernel/other/atomic.html#api-reference)
    - [Floating Point Services](https://docs.zephyrproject.org/latest/reference/kernel/other/float.html#api-reference)
    - [Version](https://docs.zephyrproject.org/latest/reference/kernel/other/version.html#api-reference)
    - [Fatal Errors](https://docs.zephyrproject.org/latest/reference/kernel/other/fatal.html#api-reference)
- [C standard library](https://docs.zephyrproject.org/latest/reference/libc/index.html) - minimal/newlib.
- [Logging](https://docs.zephyrproject.org/latest/reference/logging/index.html)
- Memory Management
  - [Demand Paging](https://docs.zephyrproject.org/latest/reference/memory_management/demand_paging.html)
- Miscellaneous
  - Checksum
    - [CRC](https://docs.zephyrproject.org/latest/reference/misc/index.html#crc)
- Structured Data
  - [JSON](https://docs.zephyrproject.org/latest/reference/misc/index.html#json)
  - [JWT](https://docs.zephyrproject.org/latest/reference/misc/index.html#jwt)
- Data Structures
  - Single-linked list
    - [Single-linked List](https://docs.zephyrproject.org/latest/reference/data_structures/slist.html#single-linked-list-api-reference)
    - [Flagged List](https://docs.zephyrproject.org/latest/reference/data_structures/slist.html#flagged-list-api-reference)
  - [Doubly-linked List](https://docs.zephyrproject.org/latest/reference/data_structures/dlist.html#doubly-linked-list-api-reference)
  - [Multi Producer Single Consumer Packet Buffer](https://docs.zephyrproject.org/latest/reference/data_structures/mpsc_pbuf.html#usage)
  - [Balanced Red/Black Tree](https://docs.zephyrproject.org/latest/reference/data_structures/rbtree.html#red-black-tree-api-reference)
  - [Ring Buffers](https://docs.zephyrproject.org/latest/reference/data_structures/ring_buffers.html#api-reference)
- [Modbus](https://docs.zephyrproject.org/latest/reference/modbus/index.html)
- Peripherals
  - [ADC](https://docs.zephyrproject.org/latest/reference/peripherals/adc.html#api-reference)
  - [Counter](https://docs.zephyrproject.org/latest/reference/peripherals/counter.html#api-reference)
  - [Clock Control](https://docs.zephyrproject.org/latest/reference/peripherals/clock_control.html#api-reference)
  - [DAC](https://docs.zephyrproject.org/latest/reference/peripherals/dac.html#api-reference)
  - [DMA](https://docs.zephyrproject.org/latest/reference/peripherals/dma.html#api-reference)
  - [EC Host Command](https://docs.zephyrproject.org/latest/reference/peripherals/ec_host_cmd_periph.html#api-reference)
  - [EEPROM](https://docs.zephyrproject.org/latest/reference/peripherals/eeprom.html#api-reference)
  - [Entropy](https://docs.zephyrproject.org/latest/reference/peripherals/entropy.html#api-reference)
  - Flash
    - [User API](https://docs.zephyrproject.org/latest/reference/peripherals/flash.html#user-api-reference)
    - [Implementation Interface API](https://docs.zephyrproject.org/latest/reference/peripherals/flash.html#implementation-interface-api-reference)
  - [GNA](https://docs.zephyrproject.org/latest/reference/peripherals/gna.html#api-reference)
  - [GPIO](https://docs.zephyrproject.org/latest/reference/peripherals/gpio.html#api-reference)
  - [Hardware Information](https://docs.zephyrproject.org/latest/reference/peripherals/hwinfo.html#api-reference)
  - [I2C EEPROM Slave](https://docs.zephyrproject.org/latest/reference/peripherals/i2c_eeprom_slave.html#api-reference)
  - [I2C](https://docs.zephyrproject.org/latest/reference/peripherals/i2c.html#api-reference)
  - [IPM](https://docs.zephyrproject.org/latest/reference/peripherals/ipm.html#api-reference)
  - [KSCAN](https://docs.zephyrproject.org/latest/reference/peripherals/kscan.html#api-reference)
  - [LED](https://docs.zephyrproject.org/latest/reference/peripherals/led.html#api-reference)
  - [Pinmux](https://docs.zephyrproject.org/latest/reference/peripherals/pinmux.html#api-reference)
  - [PWM](https://docs.zephyrproject.org/latest/reference/peripherals/pwm.html#api-reference)
  - [PS/2](https://docs.zephyrproject.org/latest/reference/peripherals/ps2.html#api-reference)
  - [PECI](https://docs.zephyrproject.org/latest/reference/peripherals/peci.html#api-reference)
  - [Regulators](https://docs.zephyrproject.org/latest/reference/peripherals/regulators.html#api-reference)
  - [RTC](https://docs.zephyrproject.org/latest/reference/peripherals/rtc.html#api-reference)
  - [Sensors](https://docs.zephyrproject.org/latest/reference/peripherals/sensor.html#api-reference)
  - [SPI](https://docs.zephyrproject.org/latest/reference/peripherals/spi.html#api-reference)
  - [UART](https://docs.zephyrproject.org/latest/reference/peripherals/uart.html#api-reference)
  - [Watchdog](https://docs.zephyrproject.org/latest/reference/peripherals/watchdog.html#api-reference)
  - [Video](https://docs.zephyrproject.org/latest/reference/peripherals/video.html#api-reference)
  - [eSPI](https://docs.zephyrproject.org/latest/reference/peripherals/espi.html#api-reference)
- Power Management
  - [Power Management Hook Interface](https://docs.zephyrproject.org/latest/reference/power_management/index.html#power-management-hook-interface)
  - [System Power Management APIs](https://docs.zephyrproject.org/latest/reference/power_management/index.html#system-power-management-apis)
  - [Device Power Management API](https://docs.zephyrproject.org/latest/reference/power_management/index.html#device-power-management-api) - The SOC interface and application use these API to perform power management operations on the devices.
  - [Device Runtime Power Management API](https://docs.zephyrproject.org/latest/reference/power_management/index.html#device-runtime-power-management-api) - The Device Drivers use these API to perform device runtime power management operations on the devices.
- [Random Number Generation](https://docs.zephyrproject.org/latest/reference/random/index.html#api-reference)
- Resource Management
  - [On/Off Manager API](https://docs.zephyrproject.org/latest/reference/resource_management/index.html#on-off-manager)
- [Shell](https://docs.zephyrproject.org/latest/reference/shell/index.html#api-reference)
- Storage
  - [Non-Volatile Storage (NVS)](https://docs.zephyrproject.org/latest/reference/storage/nvs/nvs.html#api-reference)
  - [Disk Access](https://docs.zephyrproject.org/latest/reference/storage/disk/access.html#api-reference)
  - [Flash map](https://docs.zephyrproject.org/latest/reference/storage/flash_map/flash_map.html#api-reference)
  - [Flash Circular Buffer (FCB)](https://docs.zephyrproject.org/latest/reference/storage/fcb/fcb.html#api-reference)
  - [Stream Flash](https://docs.zephyrproject.org/latest/reference/storage/stream/stream_flash.html#api-reference)
- [Task Watchdog](https://docs.zephyrproject.org/latest/reference/task_wdt/index.html#api-reference)
- Time Utilities
  - [Representation Transformation](https://docs.zephyrproject.org/latest/reference/misc/timeutil.html#representation-transformation)
  - [Time Scale Synchronization](https://docs.zephyrproject.org/latest/reference/misc/timeutil.html#time-scale-synchronization)
- USB Device Stack
  - [USB Device Controller](https://docs.zephyrproject.org/latest/reference/usb/index.html#usb-device-controller-api)
  - [USB Device Core](https://docs.zephyrproject.org/latest/reference/usb/index.html#usb-device-core-layer-api) - Low level/High level API.
  - [HID Class Device](https://docs.zephyrproject.org/latest/reference/usb/index.html#hid-class-device-api)
- User mode
  - [Memory Domain](https://docs.zephyrproject.org/latest/reference/usermode/memory_domain.html#api-reference)
  - [Kernel object](https://docs.zephyrproject.org/latest/reference/usermode/kernelobjects.html#api-reference)
  - [System Calls](https://docs.zephyrproject.org/latest/reference/usermode/syscalls.html#apis)
- [Utilities](https://docs.zephyrproject.org/latest/reference/util/index.html)
- Settings
  - [API for general settings usage](https://docs.zephyrproject.org/latest/reference/settings/index.html#api-for-general-settings-usage)
  - [API for key-name processing](https://docs.zephyrproject.org/latest/reference/settings/index.html#api-for-key-name-processing)
  - [API for runtime settings manipulation](https://docs.zephyrproject.org/latest/reference/settings/index.html#api-for-runtime-settings-manipulation)
  - [API of backend interface](https://docs.zephyrproject.org/latest/reference/settings/index.html#api-of-backend-interface)
- [Executing Time Functions](https://docs.zephyrproject.org/latest/reference/timing_functions/index.html#api-documentation)
- Virtualization
  - [Inter-VM Shared Memory](https://docs.zephyrproject.org/latest/reference/virtualization/ivshmem.html#api-reference)

## Zephyr modules

- [zscilib Zephyr module](https://github.com/zscilib/zscilib) - Scientific computing.
- [OpenThread Zephyr module](https://github.com/zephyrproject-rtos/openthread) - OpenThread.
- [micro-ROS Zephyr module](https://github.com/micro-ROS/micro_ros_zephyr_module) - micro-ROS (ROS2).
- [Rust Zephyr module](https://github.com/tylerwhall/zephyr-rust) - Module for building a Cargo project and linking it into a Zephyr image.

## Virtualization

- [ACRN](https://projectacrn.org/)
- [QEMU](https://www.qemu.org/)

## Hardware Abstraction

- [Supported boards](https://docs.zephyrproject.org/latest/boards/index.html)

## Releases

- [Zephyr releases](https://github.com/zephyrproject-rtos/zephyr/releases)
- [Release notes](https://docs.zephyrproject.org/latest/releases/index.html)
- [GitHub Release Plan](https://github.com/zephyrproject-rtos/zephyr/projects/9)

## IDEs

- [JS IDE for Zephyr OS](https://intel.github.io/zephyrjs-ide/#/)
- [Eclipse IDE](https://www.eclipse.org/ide/)
- [PlatformIO IDE](https://docs.platformio.org/en/latest/integration/ide/pioide.html)
- [PlatformIO for CLion](https://docs.platformio.org/en/latest/integration/ide/pioide.html#platformio-for-clion)
- [PlatformIO for VSCode](https://docs.platformio.org/en/latest/integration/ide/pioide.html#platformio-for-vscode)

### VSCode extensions

- [trond-snekvik.kconfig-lang](https://marketplace.visualstudio.com/items?itemName=trond-snekvik.kconfig-lang) - Kconfig language support for the Zephyr Project in VS Code.
- [trond-snekvik.devicetree](https://marketplace.visualstudio.com/items?itemName=trond-snekvik.devicetree) - DeviceTree language support for the Zephyr project in VS Code.
- [platformio.platformio-ide](https://marketplace.visualstudio.com/items?itemName=platformio.platformio-ide) - PlatformIO for VSCode.

## Development containers

- [Zephyr Docker Images](https://github.com/zephyrproject-rtos/docker-image) - CI image / Developer image.
- [Zephyr ADA containers](https://github.com/zephyr-ada/zephyr-sdk-ada) - Containers to develop Ada programs based on Zephyr RTOS.

## Development frameworks

- [PlatformIO](https://github.com/platformio) - A professional collaborative platform for embedded development.
- [Renode](https://github.com/renode/renode) - Virtual development framework for complex embedded systems.

## Blog posts

- [Zephyr website blog posts](https://www.zephyrproject.org/category/blog/)
  - [First micro-ROS Application on Zephyr RTOS (2020-06-02)](https://www.zephyrproject.org/first-micro-ros-application-on-zephyr-rtos/)
  - [Developing Zephyr RTOS embedded applications on PlatformIO and simulating on Antmicro Renode (2020-03-16)](https://www.zephyrproject.org/developing-zephyr-rtos-embedded-applications-on-platformio-and-simulating-on-antmicro-renode/)

## Videos

- [Zephyr website - Videos](https://www.zephyrproject.org/videos/)
- [Zephyr Project Youtube channel](https://www.youtube.com/c/ZephyrProject/videos)
  - [Bluetooth on Zephyr Overview](https://www.youtube.com/watch?v=1h6Hb564cUU)
  - [ACRN Hypervisor and Zephyr RTOS for Industrial IoT Applications](https://www.youtube.com/watch?v=O9JA-agbP4Y)
  - [West Overview and Status](https://www.youtube.com/watch?v=P6s0HSZAua8)
  - [New shell and logger in Zephyr 1.14](https://www.youtube.com/watch?v=JaQhhCHLxxQ)
  - [USB support in Zephyr](https://www.youtube.com/watch?v=dJ7_aRPM4Os)
  - [Zephyr Power Management 101](https://www.youtube.com/watch?v=WXOMIXDRLBU)
  - [Demand Paging: when software is bigger than available memory](https://www.youtube.com/watch?v=vYThqzCz5RQ)
  - [Using OPC UA with Zephyr](https://www.youtube.com/watch?v=HqDxohtaFUU)
  - [A deep dive into the Zephyr 2.5 device model](https://www.youtube.com/watch?v=sWaxQyIgEBY)
  - [Machine Learning with TensorFlow Lite Micro on Zephyr](https://www.youtube.com/watch?v=vMDxmEwu51M)
  - [Real Time in the Real World, Scheduler Details for Practical Problems](https://www.youtube.com/watch?v=6PpjYa1kJ1U)
  - [Coredump: a brief introduction and demo](https://www.youtube.com/watch?v=gQRiDkxbcLM)
  - [Logging subsystem overview](https://www.youtube.com/watch?v=zCNzceP2Dzk)
  - [Developing Hardware for Zephyr](https://www.youtube.com/watch?v=h5aazhjGmMY)
  - [Using Visual Trace Diagnostics on Zephyr Applications](https://www.youtube.com/watch?v=GcUnmlewGgU)
