# Cordia Labs — V0 CAD & 3D Printed Parts

CAD models, STEP source files, and 3D printable STL files for a $1,000 dual-arm robot that folds laundry.

```
Bench Format:   IKEA Råskog utility cart platform
Arm Geometry:   SO-101 / Almond derivative
Gripper Jaws:   Integrated channel for RP-S40-ST thin-film FSR & 95A TPU contact faces
Fasteners:      M3 brass heat-set inserts (M3×4×5mm)
License:        CERN Open Hardware Licence Version 2 - Strongly Reciprocal (CERN-OHL-S-2.0)
```

---

## Licensing Philosophy (CERN-OHL-S-2.0)

We deliberately license the physical CAD and printed parts under the **CERN Open Hardware Licence Version 2 – Strongly Reciprocal (CERN-OHL-S-2.0)**:

* **Hardware as a Distribution Vehicle:** Collecting usable cloth data requires putting robots into actual commercial laundry rooms instead of confining them to a single lab. The hardware must be cheap ($1,000 target BOM) and open enough to be reproduced, repaired, and distributed widely.
* **The Moat is the Dataset:** The hardware is an acquisition platform. The defensibility lies in the multimodal dataset, contact force telemetry, and trained policy weights—not in locking down 3D printed brackets.
* **Reciprocity Requirement:** Under CERN-OHL-S-2.0, anyone—including commercial teams—can build or modify this rig, provided any modified design files and manufacturing sources are released back to the community under the same reciprocal terms.

---

## Directory Overview

```
├── stls/
│   ├── jaws/
│   │   ├── Moving_Jaw_08d.stl      # Gripper jaw with internal routing pocket for RP-S40-ST FSR
│   │   └── Wrist_Roll_08c.stl      # Reinforced wrist roll actuator coupler
│   └── cart_mounts/
│       ├── overhead_rear_cam_plate.stl # Mounting plate for top-down 720p workspace camera
│       ├── leg_clip.stl                # Clamp to secure arm bases to cart oval tubing
│       └── shell_full_preview.stl      # Complete bench plate visualization
└── step/
    └── cart_bracket.step           # Solid STEP source for cart rail brackets
```

---

## 3D Printing Specifications

### Structural Parts (Brackets, Links, Camera Plate)
* **Material:** PETG or PLA-CF (Carbon Fiber reinforced PLA) for stiffness and dimensional stability.
* **Perimeters / Walls:** 4–5 walls.
* **Infill:** 40% Gyroid or Honeycomb.
* **Layer Height:** 0.20 mm.

### Gripper Jaws & Tactile Contact Surfaces
* **Structural Jaw Core:** PETG, 100% infill near the servo horn splines.
* **Compliant Contact Face:** 95A TPU (Shore A 95) printed separately or co-extruded to provide high-friction cloth grip and evenly distribute pressure across the piezoresistive film.

---

## Fastening Hardware

* **Threaded Inserts:** Standard M3 brass heat-set inserts (OD 4.6 mm, Length 5.0 mm). Installed at 220°C using a conical soldering iron tip.
* **Screws:** M3 socket head cap screws (ISO 4762), lengths 8 mm, 12 mm, 16 mm.

---

## License

Hardware designs are licensed under the **CERN Open Hardware Licence Version 2 – Strongly Reciprocal (CERN-OHL-S-2.0)**. See [LICENSE](LICENSE) for details.
