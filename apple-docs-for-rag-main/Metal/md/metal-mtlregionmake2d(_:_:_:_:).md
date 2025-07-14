

- Metal
-  MTLRegionMake2D(\_:\_:\_:\_:) 

Function

# MTLRegionMake2D(\_:\_:\_:\_:)

Creates a 3D representation of a 2D region.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func MTLRegionMake2D(
    _ x: Int,
    _ y: Int,
    _ width: Int,
    _ height: Int
) -> MTLRegion
```

## Parameters 

`x`  

The x coordinate of the origin.

`y`  

The y coordinate of the origin.

`width`  

The width of the volume.

`height`  

The height of the volume.

## Return Value

A region whose x, y, width, and height values are as specified. The z coordinate of the region’s origin is set to `0`, and the region’s depth is set to `1`.

## See Also

### Creating Regions

init()

Initializes a new region.

init(origin: MTLOrigin, size: MTLSize)

Initializes a new region with the specified origin and size.

func MTLRegionMake1D(Int, Int) -> MTLRegion

Creates a 3D representation of a 1D region.

func MTLRegionMake3D(Int, Int, Int, Int, Int, Int) -> MTLRegion

Creates a 3D region.

