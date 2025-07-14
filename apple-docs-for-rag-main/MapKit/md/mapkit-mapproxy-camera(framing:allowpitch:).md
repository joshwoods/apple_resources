

- MapKit
- MapProxy
-  camera(framing:allowPitch:) 

Instance Method

# camera(framing:allowPitch:)

Creates a camera in the context of the map that frames the given map item.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func camera(
    framing item: MKMapItem,
    allowPitch: Bool = true
) -> MapCamera
```

## Parameters 

`item`  

The MKMapItem to frame.

`allowPitch`  

A Boolean value that indicates whether you can pitch the camera to frame the content.

## Return Value

Returns a MapCamera with the framing region and pitch you specified.

## See Also

### Creating a camera proxy

func camera(framing: MKCoordinateRegion) -> MapCamera

Creates a camera in the context of the map that frames the given coordinate region.

func camera(framing: MKMapRect) -> MapCamera

Creates a camera in the context of the map that frames the given map rectangle.

