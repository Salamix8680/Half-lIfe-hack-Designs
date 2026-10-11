# Starbie: Virtual Pet PCB

A pocket-sized virtual pet on a custom PCB. A tiny pet lives on an OLED screen,
reacts when you tilt or shake it, and senses the room's temperature and humidity.

![3D render of the board](images/pcb-3d.png)

## Features
- 0.96" 128x64 I2C OLED screen
- MPU6050 motion sensor (tilt and shake)
- DHT11 temperature and humidity sensor
- Two buttons for the menu and stats screen
- Seeed XIAO ESP32-C3 microcontroller

## How it works
Button 1 opens a radial menu and you tilt the board to choose an action.
Button 2 shows the stats screen. The pet reacts to shaking and to the room's conditions.

## Schematic
![Schematic](images/schematic.png)

## PCB layout
![PCB layout](images/pcb-layout.png)

## Pin connections
| Part | XIAO pin |
|---|---|
| OLED and MPU6050 SDA | D4 |
| OLED and MPU6050 SCL | D5 |
| DHT11 data | D1 |
| Button 1 | D2 |
| Button 2 | D3 |

## Files
- `PCB/` KiCad project (schematic, board, footprints)
- `Fabrication/` Gerbers and BOM
- `Firmware/` Arduino sketch

## Build notes
Made with KiCad as part of Half-Life Week 1. Firmware is based on the Starbie
starter code.
