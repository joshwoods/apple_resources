

- MapKit JS
-  PointsOfInterestSearchOptions 

Structure

# PointsOfInterestSearchOptions

Options that you may provide when you create a points of interest search.

MapKit JS 5.45+

``` source
dictionary PointsOfInterestSearchOptions {
 string language;
 mapkit.Coordinate center;
 number radius;
 mapkit.CoordinateRegion region;
 mapkit.PointOfInterestFilter pointOfInterestFilter;
};
```

## Topics

### Configuring fetch options

region

The region that bounds the area in which to fetch points of interest.

center

The center point of the request represented as latitude and longitude.

radius

The distance provided in meters, or the longest distance derived from the center point to the region’s bounding box.

pointOfInterestFilter

A filter that lists points of interest categories to include or exclude.

language

The language ID to use when fetching points of interest.

## See Also

### Creating a Points of Interest Search

mapkit.PointsOfInterestSearch

Creates a search object for fetching points of interest.

region

The region that bounds the area in which to fetch points of interest.

center

The center point of the request represented as latitude and longitude.

radius

The distance provided in meters, or the longest distance derived from the center point to the region’s bounding box.

pointOfInterestFilter

A filter that lists points of interest categories to include or exclude.

language

The language ID to use when fetching points of interest.

MaxRadius

The maximum distance to use from the center of the region for fetching points of interest.

