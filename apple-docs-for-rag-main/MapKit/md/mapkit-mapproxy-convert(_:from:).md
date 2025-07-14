

- MapKit
- MapProxy
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a point in the specified coordinate space to a map coordinate.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func convert(
    _ point: CGPoint,
    from space: some CoordinateSpaceProtocol
) -> CLLocationCoordinate2D?
```

## Parameters 

`point`  

The point to convert.

`space`  

The reference coordinate space for `point`.

## Return Value

Returns a CLLocationCoordinate2D; or `nil,` if the specified `point` isn’t represented by a point in the MapReader associated with a Map.

## See Also

### Converting between coordinate spaces

func convert(CLLocationCoordinate2D, to: some CoordinateSpaceProtocol) -> CGPoint?

Converts a map coordinate to a point in the specified coordinate space.

