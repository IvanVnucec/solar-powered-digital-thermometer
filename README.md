# Solar powered digital thermometer

Solar powered digital thermometer with 7-segment LCD display, working without batteries, forever.

## Idea

- No batteries
- Small solar panel
- 7 segment LCD
- Sticks on the window

## Plan

- [ ] Create a simulator first
  - simulates real system w/o the need for hardware
  - graphics in Javascript
    - C/C++ can interface Javascript with WASM
- [ ] Develop lib for LCD driver
- [ ] Develop lib for Temperature sensor
  - simple PT sensor with voltage divider is good enough
- [ ] Buy hardware
- [ ] Make breadboard circuit
- [ ] Develop PCB and Assemble components
- [ ] Test

## Hardware

- [BQ25504](https://www.ti.com/lit/ds/symlink/bq25504.pdf) - Energy harvesting module
- [KXOB22-04X3F](https://ixapps.ixys.com/DataSheet/KXOB22-04X3F_Nov16.pdf), [SM141K04TFV](https://waf-e.dubuplus.com/anysolar.dubuplus.com/techsupport@anysolar.biz/O18BEsz/DubuDisk/www/Gen3/SM141K04TFV%20DATA%20SHEET%20202105.pdf) - Small solar panels
- [STM32L010K8](https://www.st.com/en/microcontrollers-microprocessors/stm32l010k8.html)
- [74AHC595 - 8-bit serial-in/serial-out or parallel-out shift register withoutput latches](https://assets.nexperia.com/documents/data-sheet/74AHC_AHCT595.pdf)
  - [Driving a 3 Digit LCD Using 74HC595 Shift Registers From a PIC Micro-Controller](https://www.youtube.com/watch?v=0vjSf-H-FJM)
- [OD-301 - Transflective 7-Segment Character Display](https://www.digikey.com/en/products/detail/orient-display/OD-301/12089299) - only 10 pins, no need for shift registers

## Software

- [awesome-embedded-rust](https://github.com/rust-embedded/awesome-embedded-rust) - Embedded rust references
- [cortex-m-quickstart](https://github.com/rust-embedded/cortex-m-quickstart) - ARM Cortex-M Rust quickstart
- [os.phil-opp.com](https://os.phil-opp.com/) - Really good Embedded Rurst code reference
- [stm32l0 crate](https://crates.io/crates/stm32l0)
