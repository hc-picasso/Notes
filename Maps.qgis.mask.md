---
id: cpwflyz0a3ym1sjf2f7sxki
title: mask
desc: ''
updated: 1645746987968
created: 1645746700275
---
## Mask raster from vector mask

1. Check validity of vector, but if not good, Repair / fix Vector
2. Use filter in attribute table to delete unneeded features
3. For the raster, use raster calculator to bring to 'nodata' unneeded data by dividing by zero: 
   ("Band">25)*"Band" / ("Band" != 0)

