

- MapKit
- MapStyle
-  hybrid(elevation:pointsOfInterest:showsTraffic:) 

Type Method

# hybrid(elevation:pointsOfInterest:showsTraffic:)

Creates a hybrid map style that includes the elevation, point of interest, and traffic characteristics you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func hybrid(
    elevation: MapStyle.Elevation = .automatic,
    pointsOfInterest: PointOfInterestCategories = .all,
    showsTraffic: Bool = false
) -> MapStyle
```

## Parameters 

`elevation`  

One of the MapStyle.Elevation values that determines whether the map renders elevation.

`pointsOfInterest`  

A collection of PointOfInterestCategories that the map displays.

`showsTraffic`  

A Boolean value that indicates whether the map displays traffic.

## Return Value

A MapStyle with the configuration you specified.

## Discussion

Note

In watchOS, depending on rendering calculations, MapKit may render the map using the Standard map style rather than requested Hybrid or Imagery styles.

## See Also

### Creating map styles

static func imagery(elevation: MapStyle.Elevation) -> MapStyle

Creates a map style based on satellite imagery with the elevation characteristics you specify.

static func standard(elevation: MapStyle.Elevation, emphasis: MapStyle.StandardEmphasis, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a standard map style that includes the elevation, point of interest, and traffic characteristics you specify.

struct Elevation

Values you use to determine whether a map renders elevation.

struct StandardEmphasis

Values that control how the framework emphasizes map features.

