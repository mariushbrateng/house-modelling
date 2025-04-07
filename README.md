# house-modelling
This repo contains step by step tutorial on how to model your terrain in Sketchup

# How to import from høydata.no 

## Download the data
Download the map you need. It will take 2-30 minutes before you get the link from hoydedata.no
Use the config below. Unzip it after download.

<img width="321" alt="Screenshot 2025-04-07 at 20 28 41" src="https://github.com/user-attachments/assets/ef5ecec2-ed9f-40a6-89a2-ce91501d5d28" />

## Download QGIS (open source) 

## Upload Terrain into QGIS1

Add new layer by: 
<img width="668" alt="Screenshot 2025-04-07 at 20 31 17" src="https://github.com/user-attachments/assets/f693c48f-266b-4dda-bc2c-3d9bdb716ffb" />

select the .tif file from hoydedata.no

you now see a ~1GB terrain file. 

## Add your property boarder file 
Add new layer by: 
<img width="667" alt="Screenshot 2025-04-07 at 20 33 39" src="https://github.com/user-attachments/assets/60d60723-b682-4d56-b6db-297a75e3bccd" />

select /metadata/dtm1_klippefil.shp file 

## Cut the terrain file with your property 

Make sure toolbox is enabled 
<img width="325" alt="Screenshot 2025-04-07 at 20 35 48" src="https://github.com/user-attachments/assets/2cfa67e0-a8a2-4b51-a6da-1c20afa98d11" />

search for "clip", select the "clip raster by mask layer" tool
<img width="352" alt="Screenshot 2025-04-07 at 20 36 06" src="https://github.com/user-attachments/assets/8b5ff0bf-849f-4acf-ad31-78aab2a5d087" />

select the terrain-layer as input layer, and your property as mask layer
<img width="1255" alt="Screenshot 2025-04-07 at 20 36 54" src="https://github.com/user-attachments/assets/02899560-7bd6-4a39-bb3e-41afa218aac5" />

you now have a new layer "clipped" 👍

uncheck the two other layers to see it

if you get lost when zooming in, use 
<img width="402" alt="Screenshot 2025-04-07 at 20 41 14" src="https://github.com/user-attachments/assets/0913aafa-ae41-4288-abda-092022fbd627" />

## Make contours on your terrain 

in toolbox, serach for contours 

<img width="248" alt="Screenshot 2025-04-07 at 20 43 48" src="https://github.com/user-attachments/assets/2f4d7656-1fd9-4e1f-bccc-971cfbe94b63" />

run with this config: 
<img width="933" alt="Screenshot 2025-04-07 at 20 49 57" src="https://github.com/user-attachments/assets/8a0d9b0e-6d35-4ee6-adae-0da8371b0ae9" />


1,00000 = one meter between every contour

you now have a new layer "contours"

## add z value to contours 
use toolbox:
<img width="259" alt="Screenshot 2025-04-07 at 20 51 24" src="https://github.com/user-attachments/assets/1b89aee3-168b-4d28-a757-9868e819a075" />

click "ELEV"
<img width="1049" alt="Screenshot 2025-04-07 at 20 52 07" src="https://github.com/user-attachments/assets/34c0b317-cf8d-4550-abde-964a5fb469d1" />

you now have new layer "Z added"
<img width="386" alt="Screenshot 2025-04-07 at 20 52 39" src="https://github.com/user-attachments/assets/7941c8cd-3ad8-4709-9b0d-baee54358b9b" />


## export contour layer "Z added"
export with:
<img width="825" alt="Screenshot 2025-04-07 at 20 46 37" src="https://github.com/user-attachments/assets/fc261d3b-4b58-47e3-a084-6c5b61409ef3" />

and this config:
<img width="609" alt="Screenshot 2025-04-07 at 20 47 25" src="https://github.com/user-attachments/assets/96ce28cf-2815-4e61-8ff4-c5ffcb6fe209" />


## import my_contours.dxf file to sketchup 
<img width="449" alt="Screenshot 2025-04-07 at 20 54 26" src="https://github.com/user-attachments/assets/3e5c1790-7b3d-45ad-a0db-a9ba76869051" />

it should look like this 

<img width="1617" alt="Screenshot 2025-04-07 at 20 53 50" src="https://github.com/user-attachments/assets/b8506654-5340-4c02-aa92-4152e3acf456" />

double click on one contour to select one part of it 
<img width="1446" alt="Screenshot 2025-04-07 at 20 55 24" src="https://github.com/user-attachments/assets/487df5ae-d95c-41ca-b40b-683c32927eb8" />

then press "cmd + a" 

now all shoule be blue like this 
<img width="1452" alt="Screenshot 2025-04-07 at 20 55 57" src="https://github.com/user-attachments/assets/93ab054a-2734-4f4f-bbb5-e079084a8a83" />

then use sandbox to do "from contours"


<img width="605" alt="Screenshot 2025-04-07 at 20 54 53" src="https://github.com/user-attachments/assets/c53c737f-c264-4211-8fb9-926cfc0f6a07" />


result:
<img width="1620" alt="Screenshot 2025-04-07 at 21 09 05" src="https://github.com/user-attachments/assets/a763506c-8649-41b2-abb6-8a9b56640b5f" />



