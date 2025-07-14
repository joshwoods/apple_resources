

- MapKit JS
-  mapkit.MapFeatureAnnotation 

Class

# mapkit.MapFeatureAnnotation

An object that represents a map feature that the user selects.

MapKit JS 5.74+

``` source
interface mapkit.MapFeatureAnnotation
```

## Overview

MapKit JS creates a `MapFeatureAnnotation` when you set selectableMapFeatures, and when a person taps a map feature. The instance is available from the selectedAnnotation property when a person selects a map feature and MapKit JS passes it to the annotationForMapFeature delegate method.

MapKit JS removes the annotation as soon as a person deselects the map feature.

## Topics

### Annotation properties

title

The title of the feature.

featureType

A value that describes the type of place the feature represents.

pointOfInterestCategory

The point-of-interest category of the feature.

id

The Place ID referencing the feature.

color

The color of the map feature.

glyphImage

The glyph image for the feature.

selectedGlyphImage

The glyph image for the selected feature.

### Fetching places

fetchPlace

Fetches the place object associated with the map feature.

## Relationships

### Inherited By

- mapkit.PlaceAnnotation

## See Also

### Points of interest

mapkit.filterExcludingAllCategories

A value that excludes all point-of-interest categories.

mapkit.filterIncludingAllCategories

A value that includes all point-of-interest categories.

mapkit.PointOfInterestFilter

A filter for determining the points of interest to include or exclude on a map or in a local search.

mapkit.PointsOfInterestSearch

An object that fetches points of interest within a specified region.

mapkit.MapFeatureAnnotationGlyphImage

An object that describes map feature annotation images.

mapkit.PointOfInterestCategory

Point-of-interest categories.

mapkit.MapFeatureType

Values that describe the feature type of a point of interest.

