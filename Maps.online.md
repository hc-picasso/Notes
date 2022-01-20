---
id: Nha2yHo4KtJdQNGMjkVSi
title: Maps online
desc: ''
updated: 1642631310467
created: 1642436600804
---
## Notes on potential online map tools
https://openmaptiles.org/docs/  
http://www.geopackage.org/guidance/extensions/tiles_encoding_webp.html  
https://gdal.org/drivers/raster/webp.html  

https://github.com/OSGeo/gdal/issues/3437  

GitHub
feature: mbtiles webp image support · Issue #3437 · OSGeo/gdal
MBTiles supports WebP since 1.3 : mbutil supports it, and the spec says: format (string): The file format of the tile data: pbf, jpg, png, webp, or an IETF media type for other formats. But as of l...
	https://github.com/OSGeo/gdal/issues/3437

https://github.com/protomaps/PMTiles

GitHub - protomaps/PMTiles: Cloud-optimized, single-file archive format for pyramids of map tiles
Cloud-optimized, single-file archive format for pyramids of map tiles - GitHub - protomaps/PMTiles: Cloud-optimized, single-file archive format for pyramids of map tiles
	https://github.com/protomaps/PMTile

 https://protomaps.com/

Web maps made simple | Protomaps
A full stack system for making vector maps on the web with Leaflet and more In the experiments, Mapbox GL JS achieved the best overall performance on mid and high
end devices for displaying raster or vector maps, while OpenLayers was the best for raster maps on all devices. Vector-based maps are a safe bet for new Web maps, since performance is on par with raster maps on mid-end smartphones, with significant less network bandwidth requirements

https://www.mdpi.com/2220-9964/9/10/563/pdf
This paper compares the performance and network usage of three popular JavaScript Web mapping libraries for implementing a Web map using different representations for geodata, and executing on different devices. In the experiments, Mapbox GL JS achieved the best overall performance on mid and high end devices for displaying raster or vector maps, while OpenLayers was the best for raster maps on all devices. Vector-based maps are a safe bet for new Web maps, since performance is on par with raster maps on mid-end smartphones, with significant less network bandwidth requirements

https://openlayers.org
OpenMapTilesOpenMapTiles
Documentation
Learn how to work with OpenMapTiles. Section with guides and tutorials about creating, styling, hosting, serving of tiles and more. (660 kB)

https://openmaptiles.org/docs/

geopackage.org
geopackage
An asciidoc version of the GeoPackage specification for easier collaboration
GitHubGitHub
feature: mbtiles webp image support · Issue #3437 · OSGeo/gdal
MBTiles supports WebP since 1.3 : mbutil supports it, and the spec says: format (string): The file format of the tile data: pbf, jpg, png, webp, or an IETF media type for other formats. But as of l... (104 kB)
https://github.com/OSGeo/gdal/issues/3437


GitHub - protomaps/PMTiles: Cloud-optimized, single-file archive format for pyramids of map tiles
Cloud-optimized, single-file archive format for pyramids of map tiles - GitHub - protomaps/PMTiles: Cloud-optimized, single-file archive format for pyramids of map tiles (53 kB)

### convert a set of GeoTIFF files into MBTiles using gdal_translate 
https://stackoverflow.com/questions/65885109/how-to-avoid-compression-when-converting-geotiff-to-mbtiles  
- Would need to review parameters to see if webp is an image option  
- Would need to see if web map can use webp

https://gdal.org/drivers/raster/mbtiles.html#tile_formats

 ### Tile formats

MBTiles can store tiles in PNG or JPEG. Support for those tile formats depend if the underlying drivers are available in GDAL. By default, GDAL will PNG tiles.

It is possible to select the tile format by setting the creation/open option TILE_FORMAT to one of PNG, PNG8 or JPEG. When using JPEG, the alpha channel will not be stored.

PNG8 can be selected to use 8-bit PNG with a color table up to 256 colors. On creation, an optimized color table is computed for each tile. The DITHER option can be set to YES to use Floyd/Steinberg dithering algorithm, which spreads the quantization error on neighbouring pixels for better rendering (note however than when zooming in, this can cause non desirable visual artifacts). Setting it to YES will generally cause less effective compression. Note that at that time, such an 8-bit PNG formulation is only used for fully opaque tiles, as the median-cut algorithm currently implemented to compute the optimal color table does not support alpha channel (even if PNG8 format would potentially allow color table with transparency). So when selecting PNG8, non fully opaque tiles will be stored as 32-bit PNG.  

**Example**  
gdal_translate -of GTiff -co "TILED=YES" utm.tif utm_tiled.tif

	-co <NAME=VALUE>

	Many formats have one or more optional creation options that can be used to control particulars about the file created. For instance, the GeoTIFF driver supports creation options to control compression, and whether the file should be tiled.

	The creation options available vary by format driver, and some simple formats have no creation options at all. A list of options supported for a format can be listed with the –formats command line option but the documentation for the format is the definitive source of information on driver creation options. See Raster drivers format specific documentation for legal creation options for each format.
https://gdal.org/programs/gdal_translate.html

## Example of webp image
- field is 2.4 Ha 
- og image orthomosaic @ 1 cm/px,  267.6 MB/Ha
- Compressed in Photoshop using webp plugin
- 1/5 of linear pixels
- 0.65% file size reduction with 75% quality
- that's 1.75 MB/Ha



Download it to zoom in
https://netorgft1964553-my.sharepoint.com/:u:/g/personal/danielpicasso_hudsoncarbon_com/Ebrh91lXOAdFpuxD6mTzbFEBNXVZvRuimdoiT64-iZwXSQ?e=E4UCVW
![Arenal 2.4 Ha](/assets/images/arenal.webp "El Arenal 2.4 Ha")

