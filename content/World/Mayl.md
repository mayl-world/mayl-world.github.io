---
map_height_y: 2048
map_width_x: 2048
scale_pixels: 268
scale_pixels_range: 25
mapCalc1: 0
---
Welcome to **Mayl**, a captivating realm shaped by ancient conflicts, mystical forces, and the pursuit of power. In this world, two continents, the [[Northern Continent]] and the [[Southern Continent]], hold a diverse tapestry of nations and factions. Mayl's history is marked by the [[The Magus War]], a devastating conflict against the [[Sviddian Mages]], where gods intervened to bring an end to the chaos.

In the aftermath, power vacuums emerged, kingdoms fell, and new alliances formed. The tensions with [[Laudia]] set the stage for the [[Sundering War]]. Magic, now permitted in [[Laudia]], became a catalyst for the global conflict, leading to an offensive strategy by Laudia and [[Ibestia]]. As you venture through Mayl's enchanting landscapes and encounter its rich cultures, prepare to navigate political intrigue, uncover ancient mysteries, and shape the fate of this extraordinary world.


```leaflet  
id: MaylFull ### Must be unique with no spaces  
image: [[The realm with Borders.png]] ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [6368, 5918]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 50% ### Size of the leaflet embed in px on your screen  
width: 100% ### Size of the leaflet embed in your note  
lat: 3150 ### To center the map, make this half of the map height.  
long: 2900 ### To center the map, make this half of the map width.  
minZoom: -5 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 1 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -1 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.5 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.09328358208955223 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: false 

```

> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`
