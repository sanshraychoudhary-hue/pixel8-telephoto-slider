# 🖨️ 3D Printing Guide — Pixel 8 Telephoto Slider

Precision tolerances are vital for smooth linear sliding and zero play in the optical axis. This guide details recommended printing technologies, materials, and slicer settings.

---

## 1. Printing Technology Comparison

| Technology | Recommendation | Why? |
| :--- | :---: | :--- |
| **SLA / DLP Resin** | **⭐ Highly Recommended** | Delivers sub-0.05 mm layer precision, glass-smooth dovetail tracks, and zero layer-line friction. Ideal for tight tolerances. |
| **FDM (Filament)** | **✔️ Good (Requires Calibration)** | Viable with a 0.2 mm or 0.4 mm nozzle. Requires careful seam placement and light wet-sanding inside the sliding grooves. |

---

## 2. Material Selection

* **Best Choice (Resin):** **ABS-Like / Tough 2000 Resin** (e.g., Anycubic ABS-Like v2, Siraya Tech Fast Mecha, or Elegoo ABS-Like). Standard budget resin can be brittle when snapped onto the visor lips.
* **Best Choice (FDM):** **PETG or ASA/ABS**. 
  > ⚠️ **Avoid standard PLA** for everyday phone use: car dashboards or warm summer pockets can easily exceed PLA's heat deflection temperature (55°C), causing warpage.

---

## 3. Recommended Slicer Profiles

### Resin (SLA / DLP / MSLA)
* **Layer Height:** `0.05 mm` (or `0.03 mm` for ultra-fine tracks)
* **Orientation:** 
  * Angle the **Visor Rail Mount** at **30°–45°** relative to the build plate.
  * Angle the **Lens Carriage** at **45°**, with the cylindrical lens bore pointing upward.
  * **Crucial:** Ensure **no support pillars generate inside the C-channel guide slots**.
* **Exposure:** Calibrate with an exposure test (Cones of Calibration) to prevent over-curing and dimension blooming inside the slots.
* **Post-Curing:** Wash thoroughly in 99% IPA (10–12 min) and cure under 405nm UV for 3–5 min. Avoid over-curing to maintain impact elasticity.

### FDM (PrusaSlicer / Bambu Studio / Cura)
* **Nozzle Diameter:** `0.4 mm` (or `0.2 mm` if available)
* **Layer Height:** `0.12 mm` (High Detail)
* **Wall Loops / Perimeters:** `4` (Ensures solid rails with no hollow voids)
* **Infill:** `40%–100%` Gyroid or Grid
* **Seam Position:** **Rear / Aligned** (keep seams on the outside exterior, never along the sliding internal faces)
* **Orientation:** Print the rail flat on its back face with supports enabled for the snap overhangs.

---

## 4. Post-Processing & Smoothing

1. **Groove Deburring:** Inspect the sliding grooves with an exacto blade or needle file to remove any microscopic brim burrs or support nubs.
2. **Fit Test:** Slide the carriage through the rail dry before installing magnets or optics. It should glide effortlessly with zero sticking.
3. **Wet Sanding:** If slight resistance is felt, wet sand the inner contact rails with **1000-grit wet sandpaper** wrapped around an ice pop stick or flat rod.
4. **Dry Lubrication:** Apply 1–2 drops of dry PTFE/silicone spray or rub candle wax/paraffin along the track. Wipe off excess.
