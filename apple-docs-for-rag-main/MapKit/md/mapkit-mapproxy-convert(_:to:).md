

- MapKit
- MapProxy
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a map coordinate to a point in the specified coordinate space.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func convert(
    _ coordinate: CLLocationCoordinate2D,
    to space: some CoordinateSpaceProtocol
) -> CGPoint?
```

## Parameters 

`coordinate`  

The map coordinate to find the corresponding point for.

`space`  

The reference coordinate space for the returned point.

## Return Value

Returns a CGPoint; otherwise `nil`, if `coordinate` isn’t represented by a point in the MapReader associated with a Map.

## See Also

### Converting between coordinate spaces

func convert(CGPoint, from: some CoordinateSpaceProtocol) -> CLLocationCoordinate2D?

Converts a point in the specified coordinate space to a map coordinate.

