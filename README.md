# DIY 3D Printer Project

A comprehensive guide for building your own 3D printer from scratch.

## Tech Stack

### Hardware Components

#### Mechanical Parts
- **Frame & Structure**
  - Aluminum extrusions (20x20mm or 20x40mm profiles)
  - Corner brackets and T-nuts
  - Lead screws (8mm diameter, 2mm pitch) for Z-axis
  - Linear rods (8mm or 10mm diameter) for X, Y, Z axes
  - Linear bearings (LM8UU or LM10UU)
  - GT2 timing belts and pulleys (20 teeth)
  - Ball bearings (608ZZ or 624ZZ)

- **Print Bed**
  - Heated aluminum bed (200x200mm or 300x300mm)
  - Borosilicate glass plate or PEI sheet
  - Bed leveling springs
  - Thermal insulation (cork sheet or silicone mat)

- **Extruder & Hotend**
  - E3D V6 hotend or similar (all-metal recommended)
  - PTFE tube (Bowden setup) or direct drive extruder
  - Nozzles (0.4mm standard, various sizes available)
  - Cooling fan for part cooling (5015 blower fan)
  - Hotend cooling fan (40mm fan)
  - Filament drive gear

#### Electronics

- **Main Controller**
  - Arduino Mega 2560 + RAMPS 1.4/1.5/1.6 board
  - OR Raspberry Pi + compatible HAT
  - OR 32-bit boards (SKR Mini E3, Duet, etc.)

- **Stepper Motors**
  - NEMA 17 stepper motors (1.8° step angle)
  - Quantity: 5 motors (X, Y, Z, Z2/dual Z, Extruder)

- **Stepper Drivers**
  - A4988 or DRV8825 drivers
  - OR TMC2208/TMC2209 (silent drivers with stallGuard)

- **Power Supply**
  - 12V or 24V DC power supply (250W-350W minimum)
  - Power switch
  - Fuse holder

- **Sensors & Switches**
  - Endstops (mechanical or optical) - 3-6 pieces
  - Thermistors (100K NTC) - 2 pieces (hotend and heated bed)
  - Auto bed leveling sensor (BLTouch, CR Touch, or inductive probe) - optional
  - Filament runout sensor - optional

- **Display & Interface**
  - LCD display (12864 or 2004)
  - Rotary encoder or SD card reader
  - Emergency stop button

- **Wiring & Connectors**
  - Heat-resistant silicone wires (18-22 AWG)
  - Connectors (JST, Dupont, XT60)
  - Cable management (spiral wrap, cable chains)
  - Heat shrink tubing

#### Tools Required for Assembly
- Hex key set (metric)
- Screwdrivers (Phillips and flathead)
- Wire strippers and crimpers
- Multimeter
- Soldering iron and solder
- Calipers (digital recommended)

### Software Stack

#### Firmware
- **Marlin Firmware** (most popular, open-source)
  - Version: 2.x recommended
  - Configuration for specific hardware setup
  - Features: auto-leveling, thermal protection, PID tuning
- **Klipper** (alternative, runs on Raspberry Pi)
- **RepRap Firmware** (for Duet boards)

#### 3D Modeling & Design
- **CAD Software**
  - Fusion 360 (free for hobbyists)
  - FreeCAD (open-source)
  - Tinkercad (beginner-friendly, web-based)
  - Blender (for complex models)
  - OpenSCAD (parametric, code-based)

#### Slicing Software
- **PrusaSlicer** (highly recommended, feature-rich)
- **Cura** (beginner-friendly, widely used)
- **Simplify3D** (paid, professional features)
- **SuperSlicer** (PrusaSlicer fork with extra features)
- **OrcaSlicer** (modern, feature-packed)

#### Printer Control & Monitoring
- **OctoPrint** (web-based printer control)
  - Runs on Raspberry Pi
  - Plugins for camera monitoring, print time estimation
- **Pronterface/Printrun** (direct USB control)
- **Repetier-Host** (alternative host software)
- **Mainsail** or **Fluidd** (for Klipper)

#### Calibration Tools
- **Teaching Tech Calibration** (web-based calibration guide)
- **PID Autotune** (built into firmware)
- **E-steps calibration** tools
- **Temperature tower** and **retraction tower** test prints

#### Development & Configuration
- **Arduino IDE** (for Marlin firmware compilation)
- **PlatformIO** (modern alternative to Arduino IDE)
- **Visual Studio Code** (with PlatformIO extension)
- **Git/GitHub** (version control for configurations)

#### File Formats
- **STL** - Standard model format for 3D printing
- **OBJ** - Alternative 3D model format
- **STEP/IGES** - CAD exchange formats
- **G-code** - Machine instruction language
- **3MF** - Advanced model format with metadata

### Operating Systems
- **Windows** (10/11) - Full compatibility with all software
- **Linux** (Ubuntu, Debian) - Excellent for OctoPrint and Klipper
- **macOS** - Compatible with most slicers and tools

### Optional Enhancements
- **Webcam** (for remote monitoring via OctoPrint)
- **Raspberry Pi** (for OctoPrint or Klipper)
- **LED lighting** (for better visibility and time-lapse)
- **Enclosure** (for temperature stability and safety)
- **Air filtration system** (for ABS and other materials)
- **UPS/Power backup** (to prevent print failures)

## Getting Started

1. **Plan Your Build**
   - Decide on print volume and frame type (Cartesian, CoreXY, Delta)
   - Source all hardware components
   - Download and review assembly guides

2. **Assembly**
   - Build the frame and install linear motion components
   - Mount stepper motors and electronics
   - Wire all components according to wiring diagram
   - Install hotend and extruder

3. **Software Setup**
   - Flash firmware to controller board
   - Configure firmware for your specific hardware
   - Install slicing software on computer
   - Set up OctoPrint (optional)

4. **Calibration**
   - Level the print bed
   - Calibrate E-steps
   - Run PID tuning for hotend and bed
   - Print calibration models

5. **First Print**
   - Start with simple test prints
   - Fine-tune settings based on results
   - Enjoy your custom 3D printer!

## Resources

- [Marlin Firmware Documentation](https://marlinfw.org/)
- [Klipper Documentation](https://www.klipper3d.org/)
- [OctoPrint](https://octoprint.org/)
- [Thingiverse](https://www.thingiverse.com/) - Free 3D models
- [Printables](https://www.printables.com/) - Free 3D models
- [RepRap Wiki](https://reprap.org/) - DIY 3D printer knowledge base
- [Teaching Tech YouTube Channel](https://www.youtube.com/c/TeachingTech) - Calibration guides

## License

This project documentation is provided as-is for educational purposes.

## Contributing

Contributions, suggestions, and improvements are welcome! Feel free to open an issue or submit a pull request.
