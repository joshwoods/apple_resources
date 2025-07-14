

- MapKit JS
- mapkit.PointsOfInterestSearch
-  mapkit.PointsOfInterestSearch 

Initializer

# mapkit.PointsOfInterestSearch

Creates a search object for fetching points of interest.

MapKit JS 5.45+

``` source
new mapkit.PointsOfInterestSearch();
```

## Discussion

To use search, create an instance of a mapkit.PointsOfInterestSearch. When you initialize a search, you can optionally set properties of the search object by providing a dictionary of PointsOfInterestSearchOptions.

## See Also

### Creating a Points of Interest Search

PointsOfInterestSearchOptions

Options that you may provide when you create a points of interest search.

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

