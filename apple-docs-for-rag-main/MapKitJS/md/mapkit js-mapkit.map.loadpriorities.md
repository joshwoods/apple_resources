

- MapKit JS
-  mapkit.Map.LoadPriorities 

Enumeration

# mapkit.Map.LoadPriorities

Values for prioritizing the visibility of specific map features while the map is loading.

MapKit JS 5.75+

``` source
interface mapkit.Map.LoadPriorities {
 const string LandCover;
 const string PointsOfInterest;
 const null None;
};
```

## Topics

### Prioritizations

LandCover

Prioritizes loading of the map land cover and borders, without POIs or labels.

PointsOfInterest

Prioritizes loading of the full standard map, with rendered POIs.

None

Signifies no preferences over what to prioritize when loading the map.

## See Also

### Prioritizing feature loading

loadPriority

A value MapKit JS uses for prioritizing the visibility of specific map features before the underlaying map tiles.

