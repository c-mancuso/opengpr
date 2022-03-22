# opengpr
## Summary
Framework for processing ground penetrating radar (GPR) and saving it as 2D profiles and block models in SEGY format.

3D visualisations depicted in this project displayed in Geoscience Analyst [Viewer](https://mirageoscience.com/mining-industry-software/geoscience-analyst/) (Mira Geoscience), a free and comprehensive geophysical model visualisation platform.

## Prerequisites
- A Unix based operating system (i.e., Linux)
- [Seismic Unix](https://github.com/JohnWStockwellJr/SeisUnix/wiki#installation-notes), a free and mature seismic data processing platform

## Data format
To date, opengpr is configured to read GPR data in:
- Sensors & Software (.DT1 & .HD)
- Seismic Unix (.su)
- SEGY (.sgy, .segy)

Final outputs are in SEGY format to be compatible with common data visualisation programs supporting seismic formats (e.g., [openDtect](https://www.dgbes.com/), [ParaView](https://www.paraview.org/), [Geoscience Analyst](https://mirageoscience.com/mining-industry-software/geoscience-analyst/), etc.)

## Examples

