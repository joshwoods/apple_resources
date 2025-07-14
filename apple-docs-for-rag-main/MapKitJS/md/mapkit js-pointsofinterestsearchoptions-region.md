

- MapKit JS
- PointsOfInterestSearchOptions
-  region 

Instance Property

# region

The region that bounds the area in which to fetch points of interest.

MapKit JS 5.45+

``` source
attribute mapkit.CoordinateRegion region;
```

## Discussion

The system determines the region from the provided bounding box or derives the region from a box enclosing the circle specified by center and radius.

## See Also

### Configuring fetch options

center

The center point of the request represented as latitude and longitude.

radius

The distance provided in meters, or the longest distance derived from the center point to the region’s bounding box.

pointOfInterestFilter

A filter that lists points of interest categories to include or exclude.

language

The language ID to use when fetching points of interest.

