

- MapKit
- MapStyle
-  imagery(elevation:) 

Type Method

# imagery(elevation:)

Creates a map style based on satellite imagery with the elevation characteristics you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func imagery(elevation: MapStyle.Elevation = .automatic) -> MapStyle
```

## Parameters 

`elevation`  

One of the MapStyle.Elevation values that determines how the map renders elevation.

## Return Value

A MapStyle with the elevation style you specified.

## Discussion

Note

In watchOS, depending on rendering calculations, MapKit may render the map using the Standard map style rather than requested Hybrid or Imagery styles.

## See Also

### Creating map styles

static func hybrid(elevation: MapStyle.Elevation, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a hybrid map style that includes the elevation, point of interest, and traffic characteristics you specify.

static func standard(elevation: MapStyle.Elevation, emphasis: MapStyle.StandardEmphasis, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a standard map style that includes the elevation, point of interest, and traffic characteristics you specify.

struct Elevation

Values you use to determine whether a map renders elevation.

struct StandardEmphasis

Values that control how the framework emphasizes map features.

