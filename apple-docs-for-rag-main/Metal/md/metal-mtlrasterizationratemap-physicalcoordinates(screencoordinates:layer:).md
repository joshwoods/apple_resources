

- Metal
- MTLRasterizationRateMap
-  physicalCoordinates(screenCoordinates:layer:) 

Instance Method

# physicalCoordinates(screenCoordinates:layer:)

Converts a point in logical viewport coordinates to the corresponding physical coordinates in a render layer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func physicalCoordinates(
    screenCoordinates: MTLCoordinate2D,
    layer layerIndex: Int
) -> MTLCoordinate2D
```

**Required**

## Parameters 

`screenCoordinates`  

A point in viewport coordinates.

`layerIndex`  

The index of the rate map to use.

## Return Value

A point in the layer’s physical coordinate system corresponding to the source point.

## Discussion

The returned coordinates are always less than or equal to the input coordinates because the rasterization rate never exceeds 1:1 in any region.

## See Also

### Converting Between Viewport and Physical Coordinates

func screenCoordinates(physicalCoordinates: MTLCoordinate2D, layer: Int) -> MTLCoordinate2D

Converts a point in physical coordinates inside a layer to its corresponding logical viewport coordinates.

**Required**

