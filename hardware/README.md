# Hardware Integration

Scripts for connecting Forge to physical tools.

## Planned

### 3D Printer (FDM)
- `stl-from-description.py` -- describe a broken part, get a printable STL
- Works with any slicer (PrusaSlicer, Cura, OrcaSlicer)
- Target: sub-$200 printers (Ender 3, Bambu A1 Mini)

### CNC Router
- `cut-template.py` -- generate G-code for common repair templates
- Flat gaskets, brackets, shims from plywood/acrylic
- Target: sub-$300 CNC (3018 Pro, Sainsmart)

### Arduino/ESP32
- `solar-monitor.ino` -- monitor solar panel voltage/current
- `water-level.ino` -- tank level sensor for rainwater collection
- All use <$5 sensors from local electronics shops

## Contributing

Build something that connects Forge to the physical world? PRs welcome.
