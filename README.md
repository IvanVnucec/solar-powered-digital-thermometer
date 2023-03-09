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
- [bq25570](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwipkpfaq879AhWhTOUKHSoaA-oQFnoECBUQAQ&url=https%3A%2F%2Fwww.ti.com%2Fproduct%2FBQ25570&usg=AOvVaw0hm_ryt7VxZQO9Xsd7HfMh) - Energy harvesting module
