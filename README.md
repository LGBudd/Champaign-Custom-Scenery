# Champaign-Custom-Scenery
FlightGear NLCD Scenery for Champaign (KCMI) and Bloomington (KBMI) areas and northern Illinois

## License

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.

## Champaign and Bloomington Areas Custom Scenery

Custom scenery for the Champaign (KCMI) and Bloomington (KBMI) areas, for the FlightGear Flight Simulator. This scenery includes:
- The airports recommended as of October 2020 from the X-Plane Scenery Gateway.
- The area between the following coordinates: 
  - min lat 40.0
  - max lat 41.1
  - min lon -88.0
  - max lon -89.0 
- Custom Material definitions and Textures for the area to make the land cover more realistic.
- Custom OSM2City scenery so it is at the correct elevation in the new scenery.
- Optional USGS orthophotos around major airports within the included area (KCMI, KBMI). 
- FlightGear Terrasync objects.

### NOTE: 
This scenery is best when used together with "Chicago and Milwaukee" and "Oshkosh and UP" custom scenery. Use of these three custom sceneries together (KORD-KMKE-Custom-Scenery, Champaign-Custom-Scenery and KOSH-KATW-KGRB_and_UP_Mich) will minimize issues at the scenery borders. They also provide a significant North-South flight area with NLCD land cover and optional photorealistic scenery.

### Data Sources

- Airports: X-Plane Scenery Gateway: https://gateway.x-plane.com/
- Landcover: National landcover database (NLCD): https://www.usgs.gov/centers/eros/science/national-land-cover-database
- Elevation: Shuttle Radar Topology Mission 1-arc-second (SRTM-1), void-filled version: https://earthexplorer.usgs.gov/
- Rivers and waterbodies: National Hydrography Dataset (NHD): https://www.usgs.gov/core-science-systems/ngp/national-hydrography
- Buildings, roads, pylons, other objects: OpenStreetMap using osm2city: https://www.openstreetmap.org/ https://osm2city.readthedocs.io/en/latest/
- FlightGear TerraSync objects
- Orthophotos: USGS Orthophotos: https://earthexplorer.usgs.gov/ Credit: U.S. Geological Survey. Map services and data available from U.S. Geological Survey, National Geospatial Program. Color correction done by a first-time amateur.

The zip archives were created using the TerraGear and TerraGear-GUI programs developed by the FlightGear project. The file repository on Google Drive includes the source data.

### To Download
**Note** that the file ChampaignSourceCode.zip is quite large in size but is NOT NEEDED for the scenery, only for further development should that be desired. It is not not needed unless you are a developer. 

The Champaign custom scenery files are available for download at the following link https://drive.google.com/drive/folders/1z4q4tOZ4zvmcKGquuYXUBBVO6AJ_FdhA?usp=sharing. There you can download the following zip archives: Buildings.zip, Objects.zip, Pylons.zip, Roads.zip, Details.zip, Terrain.zip and (optionally) Orthophotos.zip. You may also download custom materials definitions and textures in the file Illinois-data.zip, which should help make the scenery more realistic.

## Installation

To install:
1.  Create a directory on your local hard drive
1.  Download Buildings.zip, Objects.zip, Pylons.zip, Roads.zip, Details.zip, Terrain.zip, and Orthophotos,zip 
1.  Extract the files into the local directory you've created. For example, create a directory called "Champaign" on your computer. Extract the downloaded files into this directory. 
1.  Add this directory to Additional Scenery Folders in the FlightGear GUI (launcher)
1.  If you previously installed KORD-KMKE_Custom_Scenery skip to step 6, as you've already done this. Otherwise, to use the custom materials definitions and custom textures:
    1.  Download Illinois-data.zip and extract it. Rename the folder to "data.zip".
    1.  Copy this "data" folder, open "$FG_ROOT" and paste. In Windows, this is the data folder within the FlightGear $FG_ROOT directory. This should result in Illinois.xml residing in the "$FG_ROOT/Materials/regions/" directory and a folder labeled "Illinois" in the "$FG_ROOT/Textures/Terrain/" directory.
    1.  Copy the following: `<region include="Materials/regions/illinois.xml"/>`
    1.  Paste the above into the "materials.xml" file within the "North America" section. 
1.  Start FlightGear. While on the start-up screen click "Add-ons". Scroll to the "Additional scenery folders" section, then click the plus (+) sign on the right side of the screen. A dialog box will pop up. Browse to the folder you created in step 1. Highlight the folder, then click "Select Folder". Confirm that the folder was added to the bottom of "Additional scenery folders". You can now highlight and move the folder to a higher priority if necessary. NOTE: If using more than one of the three sceneries mentioned in the "Champaign and Bloomington Areas Custom Scenery" section above, you must order them as follows to minimize issues at the scenery borders: KOSH-KATW-KGRB_and_UP_Mich (top), KORD-KMKE (middle), and Champaign (bottom). 
1.  Make the selections you want to use for your next flight then click "Fly", as usual.
1.  Go to View, Rendering Options and make selections to enable Pylons and power lines, Detailed roads and railways, Buildings (OpenStreetMap Data), Random Scenery Objects, Autogenerated Vegetation, OpenStreetMap Trees, Vegetation Shadows, and Scenery Objects, as appropriate for good performance on your computer. 

## Screenshots

### Champaign Willard - University of Illinois KCMI (no orthophotos)
![KCMI](https://github.com/LGBudd/Champaign-Custom-Scenery/blob/main/Screenshots/KCMI.png)

### Central Illinois, Bloomington KBMI (orthophotos)
![KBMI](https://github.com/LGBudd/Champaign-Custom-Scenery/blob/main/Screenshots/KBMI.png)

