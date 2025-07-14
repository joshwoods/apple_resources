

- MapKit JS
- mapkit.CoordinateRegion
-  radius 

Instance Property

# radius

The distance provided in meters or the longest distance derived from the center point to the region’s bounding box.

MapKit JS 5.45+

``` source
readonly attribute number radius;
```

## Discussion

When fetching points of interest with a region, you may compare this value with MaxRadius to determine if this region is larger than the maximum available radius for a points of interest search.

