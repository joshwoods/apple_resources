

- MapKit JS
-  mapkit.PointOfInterestFilter 

Class

# mapkit.PointOfInterestFilter

A filter for determining the points of interest to include or exclude on a map or in a local search.

MapKit JS 5.32.2+

``` source
interface mapkit.PointOfInterestFilter
```

## Overview

You can apply a point of interest filter when you create a map (MapConstructorOptions), when you update an existing map (mapkit.Map), or when you fetch points of interest (SearchConstructorOptions).

## Topics

### Creating filters

including

Creates a point of interest filter that includes categories from a list that you provide.

excluding

Creates a point of interest filter that excludes categories from a list that you provide.

### Querying filter behavior

includingAllCategories

A filter that includes all point-of-interest categories.

excludingAllCategories

A filter that excludes all point-of-interest categories.

includesCategory

Returns a Boolean value that indicates whether the filter includes the provided point-of-interest category.

excludesCategory

Returns a Boolean value that indicates whether the filter excludes the provided point-of-interest category.

## See Also

### Points of interest

mapkit.filterExcludingAllCategories

A value that excludes all point-of-interest categories.

mapkit.filterIncludingAllCategories

A value that includes all point-of-interest categories.

mapkit.PointsOfInterestSearch

An object that fetches points of interest within a specified region.

mapkit.MapFeatureAnnotation

An object that represents a map feature that the user selects.

mapkit.MapFeatureAnnotationGlyphImage

An object that describes map feature annotation images.

mapkit.PointOfInterestCategory

Point-of-interest categories.

mapkit.MapFeatureType

Values that describe the feature type of a point of interest.

