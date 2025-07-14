

- MapKit
- MapStyle
-  hybrid 

Type Property

# hybrid

A map style that represents a satellite image of the area, including the paths of roads with their names layered on top.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static var hybrid: MapStyle { get }
```

## Discussion

Note

In watchOS, depending on rendering calculations, MapKit may render the map using the Standard map style rather than requested Hybrid or Imagery styles.

## See Also

### Map styles

static var imagery: MapStyle

A map style that represents a satellite image of the area the map displays.

static var standard: MapStyle

A map style that represents the default map presentation, which is a street map that shows the position of all roads and some road names, depending upon the zoom level of the map.

