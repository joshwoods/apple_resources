

- MapKit
- MapProxy
-  camera(framing:) 

Instance Method

# camera(framing:)

Creates a camera in the context of the map that frames the given map rectangle.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func camera(framing rect: MKMapRect) -> MapCamera
```

## Parameters 

`rect`  

The map rectangle to frame.

## Return Value

Returns a MapCamera that frames the rectangle you specified.

## See Also

### Creating a camera proxy

func camera(framing: MKCoordinateRegion) -> MapCamera

Creates a camera in the context of the map that frames the given coordinate region.

func camera(framing: MKMapItem, allowPitch: Bool) -> MapCamera

Creates a camera in the context of the map that frames the given map item.

