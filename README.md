# opengpr
## Summary
Framework for processing ground penetrating radar (GPR) and saving it as both 2D profiles and block models in SEGY format.

3D visualisations depicted in this project displayed in Geoscience Analyst [Viewer](https://mirageoscience.com/mining-industry-software/geoscience-analyst/) (Mira Geoscience), a free and comprehensive geophysical model visualisation platform.

## Prerequisites
- A Unix based operating system (i.e., Linux)
- [Seismic Unix](https://github.com/JohnWStockwellJr/SeisUnix/wiki#installation-notes), a free and mature seismic data processing platform

## Data format
To date, opengpr is configured to read GPR data in:
- Sensors & Software (.DT1 & .HD)
- Seismic Unix (.su)
- SEGY (.sgy, .segy)

Final outputs are in SEGY format to be compatible with common data visualisation programs supporting seismic formats (e.g., [opendTect](https://www.dgbes.com/), [ParaView](https://www.paraview.org/), [Geoscience Analyst](https://mirageoscience.com/mining-industry-software/geoscience-analyst/), etc.)

## Usage

openGPR is not intended to be a comprehensive processing package in and of itself, but a bridge between te GPR file formats and Seismic Unix (SU). Some knowledge of seismic and electromagnetic data processing is reccomended, and an understanding of SU and Bash scripting is required. Several 2D processing commands suitable for GPR data are available in SU, an [overview of the commands](docs/processing.md) most useful for GPR processing is summarized [here](docs/processing.md).

## Converting Sensors & Software Data to SU
For <ins>Sensors & Software</ins> formatted data, it is assumed that the GPR data was acquired in straight 2D profiles with locations in local coordinates with lines running east-west and/or north-south. To begin, it is reccomended that the raw data files be sorted into _inline_ and/or _crossline_ folders for lines running east-west and/or north-south, respectively. In each folder, copy and configure the Bash script geom_xline.sh (or geom_yline.sh) and run

```console
bash geom_xline.sh
```

## Exporting SU files to SEGY


## Examples

