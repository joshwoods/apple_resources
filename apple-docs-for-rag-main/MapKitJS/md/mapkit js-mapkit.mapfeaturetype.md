

- MapKit JS
-  mapkit.MapFeatureType 

Enumeration

# mapkit.MapFeatureType

Values that describe the feature type of a point of interest.

MapKit JS 5.74+

``` source
interface mapkit.MapFeatureType {
 const string PointOfInterest;
 const string Territory;
 const string PhysicalFeature;
};
```

## Topics

### Feature types

PhysicalFeature

A physical feature on the Earth such as a mountain range, river, or ocean basin.

PointOfInterest

A feature that describes a point of interest, such as a museum, park, or cafe.

Territory

A feature that describes a territory, such as a region or neighborhood.

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

mapkit.MapFeatureAnnotation

An object that represents a map feature that the user selects.

mapkit.MapFeatureAnnotationGlyphImage

An object that describes map feature annotation images.

mapkit.PointOfInterestCategory

Point-of-interest categories.

