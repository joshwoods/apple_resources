

- MapKit JS
- MapConstructorOptions
-  loadPriority 

Instance Property

# loadPriority

A value MapKit JS uses for prioritizing the visibility of specific map features before the underlaying map tiles.

MapKit JS 5.75+

``` source
attribute string|null loadPriority;
```

## Discussion

Use this property to optimize the map-loading experience and prioritize the visibility of specific map features. The available prioritization options are:

- LandCover — Prioritizes loading of the map land cover and borders, without points of interest (POIs) or labels. This is the default.

- PointsOfInterest — Prioritizes loading of the full standard map, with rendering of POIs.

- None — Signifies no preferences over what to prioritize when loading the map.

## See Also

### Setting the loading priority

mapkit.Map.LoadPriorities

Values for prioritizing the visibility of specific map features while the map is loading.

