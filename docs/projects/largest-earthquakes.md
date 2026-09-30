# 10 Largest Earthquakes (2000–2020)

![10 Largest Earthquakes (2000-2020) world map](../assets/images/project1-cover.png)

## Overview

A thematic world map of the 10 largest earthquakes from 2000 to 2020, built in QGIS from the NOAA significant earthquake database. Circle sizes show the death toll, and the map is overlaid on global active faults to show how the deadliest events relate to tectonic boundaries.

**Study Area:** Global    
**Role:** Solo project  
**Status:** Completed

---

## Methods & Tools

**Data Sources**

- Significant Earthquake Database: National Centers for Environmental Information (NCEI), NOAA
- GEM Global Active Faults Database (GEM GAF-DB)
- Land polygons: Natural Earth

**Processing Steps**

1. Loaded the significant earthquake, fault, and land layers and reprojected the map to the Equal Earth projection.
2. Used Select by Attribute to pick the 10 largest earthquakes by magnitude for 2000–2020.
3. Styled the selected events as proportional circles scaled by death toll, with all other significant earthquakes shown as small red points and faults as thin lines.
4. Wrote QGIS expressions to build the callout labels showing location and death toll for each event.
5. Composed the final layout in the Print Layout with a title, legend, data sources, and credits.

**Tools Used**

| Tool | Purpose |
|------|---------|
| QGIS | Data processing, symbology, and map layout |
| Select by Attribute | Filtering the 10 largest earthquakes by magnitude |
| QGIS expressions | Generating the callout labels |
| Equal Earth projection | Area-preserving world map display |

---

## Key Findings

- The deadliest of the 10 events was the Haiti earthquake (316,000 deaths), followed by Sumatra, Indonesia (227,899 deaths).
- These two events account for about 68% of the roughly 796,000 deaths across all 10 earthquakes.
- 9 of the 10 events occurred in Asia, and three of them were in Indonesia (Sumatra, Java, and Sulawesi).
- Many of the largest events cluster along major fault zones, notably the Himalayan region and the Indonesian archipelago.

---

## Links

[View Data Source (NOAA NCEI)](https://www.ngdc.noaa.gov/hazel/view/hazards/earthquake/search){ .md-button }
[View Fault Database (GEM GAF-DB)](https://github.com/GEMScienceTools/gem-global-active-faults){ .md-button }