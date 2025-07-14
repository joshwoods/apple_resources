

- MapKit
-  MapStyle 

Structure

# MapStyle

A style that you can apply to a map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
struct MapStyle
```

## Topics

### Creating map styles

static func hybrid(elevation: MapStyle.Elevation, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a hybrid map style that includes the elevation, point of interest, and traffic characteristics you specify.

static func imagery(elevation: MapStyle.Elevation) -> MapStyle

Creates a map style based on satellite imagery with the elevation characteristics you specify.

static func standard(elevation: MapStyle.Elevation, emphasis: MapStyle.StandardEmphasis, pointsOfInterest: PointOfInterestCategories, showsTraffic: Bool) -> MapStyle

Creates a standard map style that includes the elevation, point of interest, and traffic characteristics you specify.

struct Elevation

Values you use to determine whether a map renders elevation.

struct StandardEmphasis

Values that control how the framework emphasizes map features.

### Map styles

static var hybrid: MapStyle

A map style that represents a satellite image of the area, including the paths of roads with their names layered on top.

static var imagery: MapStyle

A map style that represents a satellite image of the area the map displays.

static var standard: MapStyle

A map style that represents the default map presentation, which is a street map that shows the position of all roads and some road names, depending upon the zoom level of the map.

## See Also

### Essentials

struct Map

A view that displays an embedded map interface.

