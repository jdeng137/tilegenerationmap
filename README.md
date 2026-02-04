# Seattle Fire Stations Tile Generation Map

## Introduction
This project creates an interactive web map that visualizes fire stations across Seattle using multiple custom tile layers. The map demonstrates the process of tile generation and layer management through four distinct tilesets, each serving a different cartographic purpose. Users can toggle between different map styles and data layers to explore various visualization approaches for geographic data.

## Map Access
**Web Map URL:** [https://jdeng137.github.io/tilegenerationmap/](https://jdeng137.github.io/tilegenerationmap/)

## Screenshots

### Tileset 1: Custom Basemap
![Custom Basemap Layer](img/tileset1.png)
*Custom designed basemap showing Seattle's street network and geographic features.*

### Tileset 2: Thematic Layer (Fire Stations Only)
![Fire Stations Thematic Layer](img/tileset2.png)
*Thematic layer displaying only fire station locations without basemap context.*

### Tileset 3: Combined Layer (Basemap + Fire Stations)
![Combined Basemap and Fire Stations](img/tileset3.png)
*Integrated layer combining the custom basemap with fire station data.*

### Tileset 4: Themed Mapbox Layer
![Themed Map Layer](img/tileset4.png)
*Stylized themed map with enhanced visual design and fire station markers.*

## Geographic Area
**Examined Region:** Seattle, Washington, United States

**Center Coordinates:** -122.31987°W, 47.59379°N

**Coverage Area:** [INSERT SPECIFIC COVERAGE AREA - e.g., "Greater Seattle metropolitan area including downtown, Capitol Hill, Queen Anne, Ballard, and surrounding neighborhoods"]

**Spatial Extent:** [INSERT BOUNDING BOX COORDINATES if known]

## Available Zoom Levels

### Tileset 1: Custom Basemap
- **Zoom Range:** [INSERT ZOOM RANGE - e.g., "Zoom levels 10-16"]
- **Optimal Viewing:** [INSERT OPTIMAL ZOOM - e.g., "Zoom level 12-14"]

### Tileset 2: Thematic Layer (Fire Stations Only)
- **Zoom Range:** [INSERT ZOOM RANGE]
- **Optimal Viewing:** [INSERT OPTIMAL ZOOM]

### Tileset 3: Combined Layer
- **Zoom Range:** [INSERT ZOOM RANGE]
- **Optimal Viewing:** [INSERT OPTIMAL ZOOM]

### Tileset 4: Themed Mapbox Layer
- **Zoom Range:** [INSERT ZOOM RANGE]
- **Optimal Viewing:** [INSERT OPTIMAL ZOOM]

## Tile Set Descriptions

### Tileset 1: Custom Basemap
This tileset provides a custom-designed basemap for the Seattle area. It serves as the foundational cartographic layer, displaying essential geographic features such as streets, water bodies, parks, and neighborhood boundaries. The styling emphasizes clarity and readability, using a neutral color palette that allows overlay data to stand out. This basemap was generated to provide a unique alternative to standard commercial basemap options while maintaining professional cartographic standards.

### Tileset 2: Thematic Layer - Fire Stations Only
This thematic tileset contains only the fire station point data without any basemap context. It displays the locations of fire stations across Seattle as distinct markers or symbols. This layer is designed to be used as an overlay on top of other basemaps, allowing for maximum flexibility in map composition. The absence of background features ensures that fire station locations are the sole focus and can be easily integrated with various basemap styles depending on the use case.

### Tileset 3: Combined Layer
This tileset integrates both the custom basemap (Tileset 1) and the fire station data (Tileset 2) into a single, cohesive layer. By combining these elements during the tile generation process rather than layering them in the browser, this approach can improve rendering performance and ensure visual consistency. The fire stations are styled to contrast effectively with the basemap, making them immediately visible while maintaining the overall cartographic aesthetic of the custom basemap design.

### Tileset 4: Themed Mapbox Layer
This tileset presents a specially themed visualization that enhances the map's visual appeal and usability. It applies advanced styling techniques to both the basemap and fire station markers, potentially incorporating color schemes, custom icons, or design elements that create a distinctive look and feel. This layer demonstrates more sophisticated cartographic design principles and may include additional visual enhancements such as halos, shadows, or specialized symbology that makes the map both functional and aesthetically engaging.

## Primary Functions

**Interactive Layer Switching:**
- Toggle between four different tile layers using checkboxes
- Real-time layer visibility control
- Multiple layers can be displayed simultaneously for comparison

**Map Controls:**
- Zoom and pan navigation controls (bottom-right)
- Scale bar showing distance in imperial units (bottom-left)
- Responsive design that adapts to different screen sizes

**Default View:**
- Map loads centered on Seattle at zoom level 12
- Themed Map (Tileset 4) is visible by default
- Light Mapbox basemap provides underlying context

## Technical Implementation

**Tile Serving:**
All custom tilesets are served from local asset directories following the standard XYZ tile structure:
```
assets/tileset_{n}/{z}/{x}/{y}.png
```
Where `n` is the tileset number (1-4), `z` is the zoom level, and `x`, `y` are the tile coordinates.

**Layer Management:**
Each tileset is loaded as a raster source and added as a separate layer, allowing independent control of visibility through the layer switcher interface.

## Libraries and Technologies

- **Mapbox GL JS (v3.18.1)** - Core mapping library for interactive web map rendering
- **HTML5/CSS3** - Web interface structure and styling
- **JavaScript (ES6)** - Map functionality and interactivity

## Data Sources

- **Fire Station Data:** [INSERT DATA SOURCE - e.g., "Seattle Fire Department, City of Seattle Open Data Portal"]
- **Basemap Data:** [INSERT DATA SOURCE - e.g., "OpenStreetMap contributors"]
- **Geographic Boundaries:** [INSERT DATA SOURCE]

## Tile Generation Process

[INSERT BRIEF DESCRIPTION OF TOOLS USED - e.g., "Tiles were generated using QGIS/Mapbox Studio/Tippecanoe with custom styling parameters"]

## Acknowledgments

- Map design and tile generation for GEOG [INSERT COURSE NUMBER]
- [INSERT INSTRUCTOR NAME], University of Washington
- [INSERT ANY OTHER ACKNOWLEDGMENTS]

## AI Disclosure

[INSERT YOUR AI USAGE DISCLOSURE - e.g., "I used AI assistance (Claude/ChatGPT/GitHub Copilot) for debugging JavaScript code, optimizing layer switcher functionality, and formatting the README documentation. I did not use AI to generate the tiles or design the core cartographic elements. I understand all code implementations and can explain the tile generation process and design decisions made in this project."]