

- MapKit
- MapStyle
-  standard(elevation:emphasis:pointsOfInterest:showsTraffic:) 

Type Method

# standard(elevation:emphasis:pointsOfInterest:showsTraffic:)

Creates a standard map style that includes the elevation, point of interest, and traffic characteristics you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func standard(
    elevation: MapStyle.Elevation = .automatic,
    emphasis: MapStyle.StandardEmphasis = .automatic,
    pointsOfInterest: PointOfInterestCategories = .all,
    showsTraffic: Bool = false
) -> MapStyle
```

## Parameters 

`elevation`  

One of the MapStyle.Elevation values that determines whether the framework renders map elevation.

`emphasis`  

One of the MapStyle.StandardEmphasis values that controls how the framework emphasizes map features.

`pointsOfInterest`  

A collection of PointOfInterestCategories displayed on the map.

`showsTraffic`  

A Boolean value that indicates whether the map displays traffic.

## Return Value

A MapStyle with the configuration you specified.

## See Also

### Creating map styles

static func hybrid(elevation: MapStyle.Elevation, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a hybrid map style that includes the elevation, point of interest, and traffic characteristics you specify.

static func imagery(elevation: MapStyle.Elevation) -> MapStyle

Creates a map style based on satellite imagery with the elevation characteristics you specify.

struct Elevation

Values you use to determine whether a map renders elevation.

struct StandardEmphasis

Values that control how the framework emphasizes map features.

