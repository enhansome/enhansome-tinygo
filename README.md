# awesome-tinygo with stars

A curated list of awesome TinyGo projects. Inspired by [awesome-go](https://github.com/avelino/awesome-go) ⭐ 182,575 | 🐛 219 | 🌐 Go | 📅 2026-08-29.

**Contributing**:

* **Issues**. Please add which category you believe fits it best along with the following markdown:
  ```markdown
  * [<project name>](<project url>) - <project description>
  ```

* **Pull requests** There are no guidelines or requirements one has to meet to be added though it would be desirable the project be original.

* [Awesome TinyGo](#awesome-tinygo)
  * [Code Editing](#code-editing)
  * [Continuous Integration](#continuous-integration)
  * [Display Hardware](#display-hardware)
  * [Embedded Systems](#embedded-systems)
    * [General use](#general-use)
    * [Protocol implementations](#protocol-implementations)
    * [Instrumentation and control with sensors and actuators](#instrumentation-and-control-with-sensors-and-actuators)
  * [Encoders](#encoders)
  * [Gaming](#gaming)
  * [WebAssembly](#webassembly)
    * [WebSockets](#websockets)
    * [DOM Manipulation](#dom-manipulation)
    * [WASI and WASM Unknown](#wasi-and-wasm-unknown)
  * [Wireless Communication](#wireless-communication)

* [Awesome TinyGo Creations](#awesome-tinygo-creations)

* [Awesome Libraries](#awesome-libraries)

* [Resources](#resources)
  * [Websites](#websites)
    * [TinyGo Community](#tinygo-community)
    * [Tutorials](#tutorials)

# Awesome TinyGo

## Code Editing

* [Display Simulator](https://github.com/sago35/tinydisplay) ⭐ 40 | 🐛 0 | 🌐 Go | 📅 2025-11-13 - `tinydisplay` is a tiny display for TinyGo development.
* [VSCode](https://github.com/tinygo-org/vscode-tinygo) ⭐ 28 | 🐛 7 | 🌐 TypeScript | 📅 2024-04-28 - TinyGo support for Visual Studio Code.
* [Vim](https://github.com/sago35/tinygo.vim) ⭐ 23 | 🐛 0 | 🌐 Vim Script | 📅 2025-12-17 - TinyGo support for Vim/NeoVim.
* [bash/zsh/clink](https://github.com/sago35/tinygo-autocmpl) ⭐ 17 | 🐛 0 | 🌐 Go | 📅 2026-07-06 - Adds bash/zsh/clink auto-completion to TinyGo.
* [VSCode Plugin](https://github.com/amken3d/tinygo-toolkit) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2026-01-09 - A comprehensive TinyGo development environment for VS Code with SDK management, target selection, board browser, driver explorer, build tools, and serial monitor
* [Goland](https://plugins.jetbrains.com/plugin/16915-tinygo) - TinyGo support for Goland.

## Continuous Integration

* [TinyHCI](https://github.com/tinygo-org/tinyhci) ⭐ 21 | 🐛 1 | 🌐 Go | 📅 2026-04-18 - Test actual hardware connections for microcontrollers. It is intended to provide smoke test implementations that exercise the basic functionality for each kind of hardware interface for each supported microcontroller.
* [setup-tinygo](https://github.com/marketplace/actions/setup-tinygo) - Sets up a TinyGo environment for GitHub Actions.

## Display Hardware

* [TinyFont](https://github.com/tinygo-org/tinyfont) ⭐ 67 | 🐛 6 | 🌐 Go | 📅 2026-04-23 - Font/text package for TinyGo displays. It is heavily based on Adafruit's GFX library.
* [TinyDraw](https://github.com/tinygo-org/tinydraw) ⭐ 51 | 🐛 2 | 🌐 Go | 📅 2025-12-19 - Draw primitives on TinyGo displays. It is heavily based on the Adafruit GFX library.
* [tinygl](https://github.com/aykevl/tinygl) ⭐ 20 | 🐛 4 | 🌐 Go | 📅 2025-09-23 - The fastest and smallest Go math library for constrained environments, like microcontrollers or WebAssembly.
* [TinyTerm](https://github.com/tinygo-org/tinyterm) ⭐ 16 | 🐛 2 | 🌐 Go | 📅 2025-12-17 - Tiny graphics library for SPI connected displays.
* [SSD1306 font](https://github.com/Nondzu/ssd1306_font) ⭐ 9 | 🐛 0 | 🌐 Go | 📅 2022-08-23 - Lite SSD1306 OLED font library using TinyGo.

## Embedded Systems

### General use

* [TinyGo Drivers](https://github.com/tinygo-org/drivers) ⭐ 747 | 🐛 155 | 🌐 Go | 📅 2026-08-21 - Provides a collection of hardware drivers for devices such as sensors and displays that can be used together with TinyGo.
* [mm-go](https://github.com/joetifa2003/mm-go) ⭐ 194 | 🐛 1 | 🌐 Go | 📅 2025-01-05 - Generic manual memory management for golang.
* [periph/devices](https://github.com/periph/devices) ⭐ 113 | 🐛 11 | 🌐 Go | 📅 2026-07-21 - Device drivers.
* [tinymath](https://github.com/orsinium-labs/tinymath) ⭐ 101 | 🐛 0 | 🌐 Go | 📅 2026-06-02 - The fastest and smallest Go math library for constrained environments, like microcontrollers or WebAssembly.
* [go-pico](https://github.com/djthorpe/go-pico) ⭐ 70 | 🐛 7 | 🌐 Go | 📅 2022-11-20 - Raspberry Pi RP2040 Pico SDK for golang.
* [go-maquina](https://github.com/soypat/go-maquina) ⭐ 58 | 🐛 0 | 🌐 Go | 📅 2023-08-25 - Finite State Machine (FSM) implementation with simplicity and maintainability in mind using Go generics.
* [pio](https://github.com/tinygo-org/pio) ⭐ 51 | 🐛 11 | 🌐 Go | 📅 2026-08-03 - Programmable I/O API for RP2040/RP2350 using TinyGo
* [tinyfs](https://github.com/tinygo-org/tinyfs) ⭐ 46 | 🐛 7 | 🌐 C | 📅 2026-02-26 - Embedded filesystems for TinyGo like FATfs and LittleFS on microcontrollers.
* [tinytest](https://github.com/orsinium-labs/tinytest) ⭐ 35 | 🐛 0 | 🌐 Go | 📅 2024-03-02 - The only assertion library that works with TinyGo
* [fat](https://github.com/soypat/fat) ⭐ 18 | 🐛 0 | 🌐 Go | 📅 2026-07-13 - Filesystem implementation using the File Allocation Table in pure Go.
* [bouncer](https://github.com/eyelight/bouncer) ⭐ 8 | 🐛 1 | 🌐 Go | 📅 2023-06-21 - bouncer is a button input handler library supporting press-lengths of different durations, and debouncing.
* [schedule](https://github.com/soypat/schedule) ⭐ 0 | 🐛 0 | 🌐 Go | 📅 2023-10-08 - Event-loop scheduling library for synchronizing actions over long periods of time.

### Protocol implementations

* [gomavlib](https://github.com/bluenviron/gomavlib) ⭐ 194 | 🐛 0 | 🌐 Go | 📅 2026-08-28 - Mavlink protocol (2.0 and 1.0) implementation in Go for control and instrumentation of autonomous vehicles.
* [mlkem768](https://github.com/FiloSottile/mlkem768) ⭐ 192 | 🐛 0 | 🌐 Go | 📅 2026-02-14 - Quantum-resistant key encapsulation method ML-KEM (formerly known as Kyber) implementation in Go.
* [natiu-mqtt](https://github.com/soypat/natiu-mqtt) ⭐ 105 | 🐛 2 | 🌐 Go | 📅 2026-07-06 - A dead-simple, extensible MQTT implementation well suited for embedded systems.
* [seqs](https://github.com/soypat/seqs) ⚠️ Archived - Networking library for use on microcontrollers. Basically a more featureful LWIP.
* [peasocket](https://github.com/soypat/peasocket) ⭐ 38 | 🐛 1 | 🌐 Go | 📅 2023-01-22 - Dead-simple, extensible websocket implementation in Go.
* [ether-swtch](https://github.com/soypat/ether-swtch) ⚠️ Archived - Low level Ethernet/IP/TCP/HTTP stack marshaller/unmarshaller for use in tiny places.
* [peamodbus](https://github.com/soypat/peamodbus) ⭐ 8 | 🐛 0 | 🌐 Go | 📅 2023-11-07 - Fault tolerant, TCP modbus implementation in Go that just works. Apt for embedded systems.
* [go-bthome](https://github.com/hybridgroup/go-bthome) ⭐ 4 | 🐛 0 | 🌐 Go | 📅 2025-01-07 - Minimal package for creating and parsing BTHome service data using Go/TinyGo.
* [go-cayenne-lib](https://github.com/TheThingsNetwork/go-cayenne-lib) ⭐ 4 | 🐛 1 | 🌐 Go | 📅 2023-10-12 - CayenneLPP in Go
* [tiny-sproto](https://github.com/soypat/tiny-sproto) ⭐ 4 | 🐛 0 | 🌐 Go | 📅 2022-12-04 - A simple Point-to-Point Protocol implementation written in Go.
* [go-canard](https://github.com/soypat/go-canard) ⭐ 3 | 🐛 0 | 🌐 Go | 📅 2022-08-21 - CAN/OpenCyphal implementation in pure Go. Port of libcanard.
* [achicken](https://github.com/soypat/achicken) ⭐ 1 | 🐛 0 | 🌐 Go | 📅 2022-11-04 - Dead-simple serial protocol with CRC for small projects.

### Instrumentation and control with sensors and actuators

* [pctl](https://github.com/brandondube/pctl) ⭐ 49 | 🐛 1 | 🌐 Go | 📅 2023-09-10 - "process control" is a package for industrial control in Go. Filtering and control theory algorithms.
* [fusion](https://github.com/aykevl/fusion) ⭐ 15 | 🐛 1 | 🌐 Go | 📅 2019-07-13 - Sensor fusion algorithms (gyroscope/accelerometer) implemented in pure Go.
* [magcal](https://github.com/ysoldak/magcal) ⭐ 7 | 🐛 2 | 🌐 Go | 📅 2021-11-29 - (Magical) Magnetometer Calibration

## Encoders

* [gjson](https://github.com/tidwall/gjson) ⭐ 15,557 | 🐛 99 | 🌐 Go | 📅 2026-08-28 - Get JSON values quickly - JSON parser for Go
* [easyjson](https://github.com/mailru/easyjson) ⭐ 4,916 | 🐛 99 | 🌐 Go | 📅 2026-03-14 - Fast JSON serializer for golang.
* [jsony](https://github.com/orsinium-labs/jsony) ⭐ 174 | 🐛 0 | 🌐 Go | 📅 2025-11-20 - A blazing fast and safe Go package for serializing JSON
* [protobuf-go-lite](https://github.com/aperturerobotics/protobuf-go-lite) ⭐ 62 | 🐛 1 | 🌐 Go | 📅 2026-08-28 - Reflection-free Protobuf for Go.

## Gaming

* [koebiten](https://github.com/sago35/koebiten) ⭐ 56 | 🐛 0 | 🌐 Go | 📅 2026-08-29 - Koebiten is a 2D game engine that runs on TinyGo. Inspired by Ebitengine and is characterized by its simple API.
* [tinygba](https://github.com/tinygo-org/tinygba) ⭐ 36 | 🐛 3 | 🌐 Go | 📅 2026-02-22 - Tools and helpers for developing GBA programs using TinyGo.
* [wasm4go](https://github.com/orsinium-labs/wasm4go) ⭐ 29 | 🐛 0 | 🌐 Go | 📅 2024-03-29 - Framework for making WASM-4 games with Go (and TinyGo).
* [Flappy Boot](https://github.com/bjatkin/flappy-boot) ⭐ 26 | 🐛 3 | 🌐 Go | 📅 2024-09-02 - clone of flappy bird for the GBA written using TinyGo.
* [gonx](https://github.com/racerxdl/gonx) ⭐ 19 | 🐛 0 | 🌐 Go | 📅 2021-01-03 - Wrapper around libnx for developing Nintendo Switch programs using TinyGo.
* [firefly-go](https://github.com/firefly-zero/firefly-go) ⭐ 18 | 🐛 0 | 🌐 Go | 📅 2026-08-07 - Go SDK for making Firefly Zero games
* [tinyrogue](https://github.com/deadprogram/tinyrogue) ⭐ 13 | 🐛 0 | 🌐 Go | 📅 2026-04-04 - Fun package for creating roguelike games with TinyGo on Firefly Zero using WASM
* [ghost-castle](https://github.com/deadprogram/ghost-castle) ⭐ 1 | 🐛 1 | 🌐 Go | 📅 2025-12-26 - Simple roguelike game written using TinyGo with TinyRogue on Firefly Zero
* [Hunt the Wumpus](https://github.com/smittytone/pi-pico-go.git) ⚠️ Archived - Handheld gaming powered by the Raspberry Pi Pico and TinyGo.

## WebAssembly

### DOM Manipulation

* [TinyDom](https://github.com/Nerzal/tinydom) ⭐ 23 | 🐛 0 | 🌐 Go | 📅 2022-08-04 - DOM manipulation library. For use in WASM
* [GoUI](https://github.com/goui-org/goui) ⭐ 12 | 🐛 1 | 🌐 Go | 📅 2024-01-30 - A web framework for making user interfaces

### WebSockets

* [TinyWebSocket](https://github.com/Nerzal/tinywebsocket) ⭐ 9 | 🐛 0 | 🌐 Go | 📅 2021-03-05 - Wraps the `syscall/js` api to provide a better developer experience, while being compilable by TinyGo

### WASI and WASM Unknown

* [go-modules](https://github.com/bytecodealliance/go-modules) ⭐ 148 | 🐛 38 | 🌐 Go | 📅 2026-01-28 - WebAssembly, WASI, and Component Model tools for Go
* [wypes](https://github.com/orsinium-labs/wypes) ⭐ 25 | 🐛 0 | 🌐 Go | 📅 2025-10-03 - Go library to define type-safe host functions in wazero and other WebAssembly runtimes.
* [wasmCV](https://github.com/wasmvision/go-wasmcv) ⭐ 9 | 🐛 0 | 🌐 Assembly | 📅 2025-08-13 - Go bindings for wasmCV computer vision interfaces using WebAssembly.

## Wireless Communication

* [Go Bluetooth](https://github.com/tinygo-org/bluetooth) ⭐ 995 | 🐛 129 | 🌐 C | 📅 2026-08-26 - Go Bluetooth is a cross-platform package for using Bluetooth Low Energy hardware from the Go programming language.
* [lorawan](https://github.com/tinygo-org/drivers/tree/release/lora/lorawan) ⭐ 747 | 🐛 155 | 🌐 Go | 📅 2026-08-21 - LoRaWAN implementation for embedded devices using TinyGo.

# Awesome TinyGo Creations

**Hardware and software implementations**

* [go-haystack](https://github.com/hybridgroup/go-haystack) ⭐ 1,510 | 🐛 5 | 🌐 Go | 📅 2025-08-20 - Track personal Bluetooth devices via Apple's "Find My" network using OpenHaystack and Macless-Haystack with tools written in Go/TinyGo. No Apple hardware required!
* [wasmVision](https://github.com/wasmvision/wasmvision) ⭐ 245 | 🐛 1 | 🌐 Go | 📅 2026-02-16 - wasmVision gets you going with computer vision using WebAssembly with processors written using TinyGo/Rust/C.
* [USB HID Keyboard firmware for TinyGo](https://github.com/sago35/tinygo-keyboard) ⭐ 115 | 🐛 11 | 🌐 Go | 📅 2026-07-28 - keyboard firmware for tinygo
* [HeadTracker](https://github.com/ysoldak/HeadTracker) ⭐ 111 | 🐛 6 | 🌐 Go | 📅 2026-06-26 - Bluetooth DIY Head Tracker, for Nano 33 BLE and XIAO BLE Sense boards.
* [TinyGlobo](https://github.com/hybridgroup/tinyglobo) ⭐ 64 | 🐛 0 | 🌐 Go | 📅 2026-01-29 - A pico balloon floats into the great big world, towing a RP2040 Pico programmed with TinyGo using LoraWAN to communicate along the way.
* [Gobadge](https://github.com/tinygo-org/gobadge) ⭐ 40 | 🐛 3 | 🌐 Go | 📅 2025-08-18 - TinyGo powered badge using Adafruit Pybadge Hardware
* [Gopherbot](https://github.com/hybridgroup/gopherbot) ⭐ 23 | 🐛 3 | 🌐 Go | 📅 2025-01-15 - A robotic gopher plushie that you can code using TinyGo
* [ledrace](https://github.com/conejoninja/ledrace) ⭐ 11 | 🐛 0 | 🌐 Go | 📅 2024-10-14 - TinyGo implementation of Open LED Race
* [FPV Combat Gadget](https://github.com/ysoldak/fpvc-gadget) ⭐ 5 | 🐛 2 | 🌐 Go | 📅 2025-12-28 - [FPV Combat](https://fpv-combat.com/) configurator with display and a rotary encoder (multi-level menu system with input), runs on XIAO.
* [gopher.pretty](https://github.com/sat0ken/gopher.pretty) ⭐ 5 | 🐛 0 | 📅 2026-07-05 - Kicad footprint file of Gopher design. Lets you make your own board.
* [LED Cube](https://github.com/tinygo-org/things/tree/master/ledcube) ⭐ 2 | 🐛 0 | 🌐 Go | 📅 2025-01-13 - 6x32x32 LED cube, inspired by a LED cube I've seen at CCC and the SquareWave Dot cube.
* [Arduino Mega Programmer](https://github.com/Gustavomurta/Arduino_Mega_Programmer) ⭐ 1 | 🐛 0 | 🌐 Go | 📅 2024-02-17 - Read ROMs, EPROM, Flash of older computers such as a Commodore C128 ROM chip.
* [gopher-board](https://github.com/sat0ken/gopher-board) ⭐ 1 | 🐛 0 | 📅 2026-06-06 - Original board with Gopher design for Waveshare RP2040-Zero and XIAO.
* [RC PWM to RGB LED](https://github.com/ysoldak/pwm-ws2812) ⭐ 1 | 🐛 0 | 🌐 Go | 📅 2023-04-19 - WS2812 LED strip color and brightness control with two RC PWM channels

# Awesome Libraries

**Packages that make life easier or more awesome in TinyGo**

* [`u-root`](https://github.com/u-root/u-root) ⭐ 3,069 | 🐛 163 | 🌐 Go | 📅 2026-08-28 - Go versions of many standard Linux tools, such as ls, cp, or shutdown among other awesome OS stuff.
* [`cbor`](https://github.com/fxamacker/cbor) ⭐ 1,081 | 🐛 30 | 🌐 Go | 📅 2026-08-28 - Library for encoding and decoding Concise Binary Object Representation data and Sequences (RFC8949).
* [`mathgl`](https://github.com/go-gl/mathgl) ⭐ 609 | 🐛 9 | 🌐 Go | 📅 2024-11-03 - A pure Go 3D math library.
* [`float16`](https://github.com/x448/float16) ⭐ 99 | 🐛 5 | 🌐 Go | 📅 2026-08-23 - IEEE 754 half-precision floating-point format (binary16) library.
* [`math32`](https://github.com/chewxy/math32) ⭐ 86 | 🐛 5 | 🌐 Go | 📅 2026-05-15 - 32bit math functions in pure Go.
* [`godsp`](https://github.com/goccmack/godsp) ⭐ 39 | 🐛 1 | 🌐 Go | 📅 2020-03-14 - Basic digital signal processing functions using the discrete wavelet transform (DWT).
* [`tinystring`](https://github.com/cdvelop/tinystring) ⭐ 21 | 🐛 0 | 🌐 Go | 📅 2026-08-21 - Lightweight text manipulation library with a fluid API and no external dependencies.
* [`lap`](https://github.com/soypat/lap) ⭐ 13 | 🐛 0 | 🌐 Go | 📅 2023-07-08 - Extremely lightweight linear algebra package similar to gonum.
* [`tvd`](https://github.com/soypat/tvd) ⭐ 3 | 🐛 0 | 🌐 Go | 📅 2023-07-14 - Total Variation Denoising filter ideal for capturing edge transitions.
* [`cereal`](https://github.com/soypat/cereal) ⭐ 2 | 🐛 0 | 🌐 Go | 📅 2023-11-27 - All-you-need serial device tooling integrating bugst, goburrow, tarm and sers serial libraries.

# Resources

## Websites

### TinyGo Community

* [TinyGopher Worldmap](https://getethermap.org/m/tinygophers) - Locate Tinygophers all over the world!

### Tutorials

* [Blinky tutorial](https://github.com/tinygo-org/tinygo-site/blob/379c887947063e08bc9547a034b7ced68ab30628/content/getting-started/blinky.md) ⭐ 70 | 🐛 51 | 🌐 HTML | 📅 2026-06-24 - A tutorial to get familiar with TinyGo basics.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-29._
