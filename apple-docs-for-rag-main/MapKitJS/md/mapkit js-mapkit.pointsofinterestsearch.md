

- MapKit JS
-  mapkit.PointsOfInterestSearch 

Class

# mapkit.PointsOfInterestSearch

An object that fetches points of interest within a specified region.

MapKit JS 5.45+

``` source
interface mapkit.PointsOfInterestSearch
```

## Mentioned in 

MapKit JS 5

## Overview

Use mapkit.PointsOfInterestSearch to fetch points of interest. Mapkit JS exposes this functionality through a search object that makes network requests to the search service. To use search, create an instance of a mapkit.PointsOfInterestSearch object with the desired options and use the instance to make search requests. You may optionally specify a mapkit.PointOfInterestFilter that lists categories to include or exclude. The default behavior of the fetch returns all points of interest.

To leverage the map’s current region to request points of interest, create a request with a rectangular bounding box using a mapkit.CoordinateRegion. The request fetches points of interest within the rectangular region.

To retrieve points of interest nearby or “around the user,” create a request with a circular area defined by a center point of mapkit.Coordinate and a radius in meters.

If you set a language ID, the fetch returns addresses in the selected language, if available; for instance, `fr-CA` or `fr-FR`. If you don’t provide a language ID, the fetch request uses the language ID initialized with the map.

## Topics

### Creating a Points of Interest Search

mapkit.PointsOfInterestSearch

Creates a search object for fetching points of interest.

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

### Fetching points of interest

search

Fetches points of interest.

PointsOfInterestSearchDelegate

An object or callback function that MapKit JS calls when fetching points of interest.

PointsOfInterestSearchResponse

The result of a request used to fetch points of interest.

### Canceling a points of interest search

cancel

Cancels a search request using its request ID.

## See Also

### Points of interest

mapkit.filterExcludingAllCategories

A value that excludes all point-of-interest categories.

mapkit.filterIncludingAllCategories

A value that includes all point-of-interest categories.

mapkit.PointOfInterestFilter

A filter for determining the points of interest to include or exclude on a map or in a local search.

mapkit.MapFeatureAnnotation

An object that represents a map feature that the user selects.

mapkit.MapFeatureAnnotationGlyphImage

An object that describes map feature annotation images.

mapkit.PointOfInterestCategory

Point-of-interest categories.

mapkit.MapFeatureType

Values that describe the feature type of a point of interest.

