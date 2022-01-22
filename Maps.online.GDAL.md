---
id: Cm4S2xW62vJF6ozxqqLuh
title: GDAL
desc: ''
updated: 1642864607526
created: 1642628703479
---
https://www.youtube.com/watch?v=8iCWUp7WaTk

Open anaconda terminal as admin

Create virtual environment  

```conda create --name geo```

Activate virtual environment

```conda activate geo ```

Install gdal

```install -c conda-forge gdal```

Check GDAL installed

```python -m pip show gdal```

Install other stuff

```
from osgeo import gdal
from osgeo import ogr
from osgeo import osr
```

Should be good to go



Activate virtual environment

```conda activate geo ```
```
import gdal
import ogr
import osr
```
Should be good to go
## Just strating over

Activate virtual environment

```conda activate geo ```   
```gdal_translate --formats```
```gdal_translate --format MBTiles```
```gdal_translate --format WEBP```
C:\Users\Hudson Carbon MSI\OneDrive - hudsoncarbon.com\Desktop\BaseMap.gpkg
```
gdal_translate -of WEBP C:\GDAL\arenal.tif C:\GDAL\arenal.webp
```
Input file size is 27947, 29858  
ERROR 6: WEBP maximum image dimensions are 16383 x 16383.

**Won't be able to do it with webp**

Try tiles

gdal_translate -of MBTiles -co "TILE_FORMAT=JPEG" -lco "MAXZOOM=15" -lco ""MINZOOM"=0" C:\GDAL\arenal.tif C:\GDAL\arenal.mbtiles

gdal_translate -of MBTiles C:\GDAL\arenal.tif C:\GDAL\arenal.MBTiles
$ gdaladdo -r average C:\GDAL\arenal.MBTiles 2 4 8 16

ogr2ogr -f MBTILES  C:\GDAL\arenal.mbtiles C:\GDAL\arenal.tif -dsco MAXZOOM=10

gdal_translate -multi -wo "USE_OPENCL=TRUE" -of MBTILES  C:\GDAL\arenal.tif C:\GDAL\arenal.mbtiles 

gdalinfo C:\GDAL\arenal.mbtiles

- Maybe if I pre-tile the othomosaic, then I can batch process into webp

gdal_translate -of GTiff -co "TILED=YES" C:\GDAL\arenal.tif C:\GDAL\arenal-tiled.tif

Another solution using GDAL is the gdal_retile.py tool:
```mkdir image_tiles```
```gdal_retile.py -v -r bilinear -levels 1 -ps 20000 20000 -co "TILED=YES" -co "COMPRESS=JPEG" -targetDir image_tiles big_input_image.tif```

```gdal_retile.py -v -r bilinear -levels 1 -ps 15000 15000 -co "TILED=YES" -co -targetDir image_tiles big_input_image.tif```

```gdal_retile.bat -v -r bilinear -levels 1 -of WEBP -ps 15000 15000 -co -targetDir C:\GDAL\aaa C:\GDAL\arenal.tif ```

```gdalwarp -t_srs EPSG:3857 -r near C:\GDAL\arenal.tif  C:\GDAL\arenal2.tif```
```gdal_translate -of mbtiles C:\GDAL\arenal2.tif C:\GDAL\arenal2.mbtiles
```gdaladdo -r nearest C:\GDAL\arenal2.mbtiles 2 4 8 16