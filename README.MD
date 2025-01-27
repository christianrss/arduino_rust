avrdude -p m328p -c arduino -P COM6 -b 115200 -U flash:w:arduino_rust.elf
cargo +nightly build -Z build-std=core --target avr-atmega328p.json --release