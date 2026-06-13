# Cyclone Amphan — Cinematic GIS Visualization

![Cyclone Amphan Wind Field Animation](../assets/images/amphan.gif)

## Overview

This project recreates the complete lifecycle of Super Cyclone Amphan (2020) through a temporal wind-field animation built in QGIS using ERA5 climate reanalysis data from the Copernicus Climate Data Store. The animation traces the storm from its genesis over the Bay of Bengal through rapid intensification, landfall near the India–Bangladesh coast, and final dissipation across eastern India and Bangladesh.

The goal was to transform raw atmospheric reanalysis data into cinematic cartographic storytelling — turning meteorological records into motion, tension, and narrative.

**Study Area:** Bay of Bengal, West Bengal, Odisha, and coastal Bangladesh
**Data Source:** ERA5 Hourly Reanalysis (Copernicus Climate Data Store)
**Temporal Coverage:** May 16–21, 2020
**Role:** Solo Project
**Status:** Completed

---

## Storm Overview

Cyclone Amphan originated as a low-pressure system over the Bay of Bengal in mid-May 2020. It underwent rapid intensification and reached Super Cyclonic Storm status — one of the strongest cyclones to strike eastern India and Bangladesh in recent decades. It made landfall on **20 May 2020** near the Sundarbans delta at the India–Bangladesh border, bringing extremely severe winds and catastrophic storm surge to West Bengal, Odisha, and coastal Bangladesh.

| Parameter             | Details                                        |
| --------------------- | ---------------------------------------------- |
| Storm Category        | Super Cyclonic Storm                           |
| Peak Wind Speed       | ~270 km/h (1-minute sustained)                 |
| Landfall Date         | 20 May 2020                                    |
| Landfall Location     | Sundarbans, India–Bangladesh border            |
| Affected Regions      | West Bengal, Odisha, coastal Bangladesh        |
| Data Source           | ERA5 Hourly Reanalysis, Copernicus CDS         |

---

## Storm Lifecycle

The animation follows four distinct phases of the cyclone's evolution:

**🌀 Cyclogenesis** — Formation of a low-pressure system over the warm Bay of Bengal, with wind vectors beginning to organize into a cyclonic pattern.

**🌊 Rapid Intensification** — Explosive deepening of the storm as sea surface temperatures fuelled an accelerating vortex, intensifying from a depression to a Super Cyclonic Storm within 36 hours.

**📍 Landfall** — The eye makes landfall near the Sundarbans on 20 May 2020. Wind streamlines compress and the storm's full spatial scale becomes visible against the coastal terrain.

**🌧️ Dissipation** — Inland weakening as the cyclone lost its oceanic energy source, with wind fields gradually fragmenting across eastern India and Bangladesh.

---

## Methods & Tools

### Data Sources

* ERA5 hourly reanalysis wind data (u10 and v10 components) from the Copernicus Climate Data Store
* Custom hillshade terrain derived from a digital elevation model for cinematic basemap aesthetics

### Processing Steps

1. Downloaded ERA5 hourly wind component data (u10, v10) covering May 16–21, 2020 from Copernicus CDS.
2. Loaded GRIB files into QGIS using the Mesh Layer rendering engine for native temporal control.
3. Configured temporal animation settings to step through hourly wind snapshots.
4. Styled wind vectors and streamlines to convey speed and direction with visual clarity.
5. Designed a custom hillshade basemap for cinematic cartographic depth.
6. Exported 200+ individual frames at consistent styling across all timesteps.
7. Compiled frames into a smooth animation sequence.

### Tools Used

| Tool                     | Purpose                                              |
| ------------------------ | ---------------------------------------------------- |
| QGIS                     | Temporal animation, mesh rendering, and map styling  |
| Copernicus CDS           | ERA5 hourly reanalysis wind data acquisition         |
| GRIB Mesh Renderer       | Native GRIB file rendering with temporal playback    |
| Wind Vector Styling      | Directional streamlines and speed-mapped arrows      |
| Custom Hillshade Terrain | Cinematic basemap aesthetics                         |
| Frame Export + Compile   | 200+ exported frames assembled into animation        |

---

## Key Findings

* Successfully visualized the full lifecycle of Cyclone Amphan — from genesis to dissipation — using hourly ERA5 wind data.
* Demonstrated how raw atmospheric reanalysis datasets can be transformed into fluid, cinematic visual narratives.
* The rapid intensification phase (May 17–18) is visually striking: wind vectors accelerate and the cyclonic circulation tightens dramatically within a few frames.
* Landfall geometry closely matches historical records, validating the ERA5 data fidelity for storm reconstruction.
* The hillshade basemap adds depth and geographic context that heightens the storytelling impact.

---

## Technical Highlights

* ERA5 GRIB mesh rendering with QGIS's native temporal controller for frame-accurate playback.
* Hourly temporal resolution capturing sub-daily storm dynamics across a 5-day window.
* Wind streamline and vector styling calibrated to highlight the cyclone's rotational structure.
* 200+ frame export pipeline compiled into a smooth animation sequence.
* Cinematic cartographic design combining atmospheric data with terrain visualization.

---

## Animation Preview

<video width="100%" controls>
  <source src="../assets/videos/cyclone.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## Reflections

What fascinated me most during this project was seeing how raw atmospheric datasets could be transformed into visual storytelling. ERA5 reanalysis data is, at its core, a grid of numbers — wind speeds and directions at every point on the Earth's surface, every hour. But rendered as streamlines and vectors moving through time, those numbers became something visceral: the slow spiral of cyclogenesis, the explosive tightening of rapid intensification, the moment the eye crosses the coast.

This project sits at the intersection of my growing interests in **climate visualization**, **temporal GIS**, **environmental storytelling**, and **geospatial animation** — and it has deepened my sense of what maps can do when they move.

---

## Links

[ERA5 Dataset (Copernicus CDS)](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels){ .md-button }


