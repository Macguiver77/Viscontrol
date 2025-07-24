# Burner Control System for Arduino UNO

This project implements a state machine for controlling a burner system based on various inputs, outputs, timers, and counters. All inputs and outputs are simulated via the serial console.

## Setup Instructions

1. Open the Arduino IDE
2. Open the sketch file: `burner-control-avr/burner-control-avr.ino`
3. Select the correct board: Tools > Board > Arduino AVR Boards > Arduino Uno
4. Select the correct port: Tools > Port > [Your Arduino port]
5. Click the Upload button or press Ctrl+U (Cmd+U on Mac)

## Troubleshooting

If you encounter upload errors:

1. Make sure your Arduino UNO is properly connected
2. Verify the correct port is selected in the Arduino IDE
3. Try pressing the reset button on the Arduino just before uploading
4. Check that you have the Arduino AVR boards package installed (Tools > Board > Boards Manager)
5. Ensure the sketch is in a folder with the same name (burner-control-avr)

## Usage

Once uploaded, open the Serial Monitor (Tools > Serial Monitor) and set the baud rate to 9600. You can interact with the system using the following commands:

- `start` - Press start button
- `stop` - Press stop button
- `pcfs:on/off` - Set Primary Combustion Flame Sensor
- `scfs:on/off` - Set Secondary Combustion Flame Sensor
- `lts:value` - Set Load Temperature Sensor value
- `fts:value` - Set Flame Temperature Sensor value
- `status` - Show current system status 