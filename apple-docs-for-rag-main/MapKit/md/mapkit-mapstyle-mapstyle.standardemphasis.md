

- MapKit
- MapStyle
-  MapStyle.StandardEmphasis 

Structure

# MapStyle.StandardEmphasis

Values that control how the framework emphasizes map features.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct StandardEmphasis
```

## Topics

### Controlling the map’s emphasis

static var automatic: MapStyle.StandardEmphasis

The default level of emphasis.

static var muted: MapStyle.StandardEmphasis

A muted emphasis style, that deemphasizes the map’s imagery.

## See Also

### Creating map styles

static func hybrid(elevation: MapStyle.Elevation, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a hybrid map style that includes the elevation, point of interest, and traffic characteristics you specify.

static func imagery(elevation: MapStyle.Elevation) -> MapStyle

Creates a map style based on satellite imagery with the elevation characteristics you specify.

static func standard(elevation: MapStyle.Elevation, emphasis: MapStyle.StandardEmphasis, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a standard map style that includes the elevation, point of interest, and traffic characteristics you specify.

struct Elevation

Values you use to determine whether a map renders elevation.

