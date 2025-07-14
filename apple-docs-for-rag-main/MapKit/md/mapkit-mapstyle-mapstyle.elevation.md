

- MapKit
- MapStyle
-  MapStyle.Elevation 

Structure

# MapStyle.Elevation

Values you use to determine whether a map renders elevation.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct Elevation
```

## Topics

### Elevation styles

static var automatic: MapStyle.Elevation

The default elevation style, that renders a flat, 2D map.

static var flat: MapStyle.Elevation

A value that renders a flat, 2D map.

static var realistic: MapStyle.Elevation

A value that renders a realistic, 3D map.

## See Also

### Creating map styles

static func hybrid(elevation: MapStyle.Elevation, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a hybrid map style that includes the elevation, point of interest, and traffic characteristics you specify.

static func imagery(elevation: MapStyle.Elevation) -> MapStyle

Creates a map style based on satellite imagery with the elevation characteristics you specify.

static func standard(elevation: MapStyle.Elevation, emphasis: MapStyle.StandardEmphasis, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a standard map style that includes the elevation, point of interest, and traffic characteristics you specify.

struct StandardEmphasis

Values that control how the framework emphasizes map features.

