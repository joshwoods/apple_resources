

- Metal
-  MTLRegionMake1D(\_:\_:) 

Function

# MTLRegionMake1D(\_:\_:)

Creates a 3D representation of a 1D region.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func MTLRegionMake1D(
    _ x: Int,
    _ width: Int
) -> MTLRegion
```

## Parameters 

`x`  

The x coordinate of the origin.

`width`  

The width of the volume.

## Return Value

A region whose x and width values are as specified. The y and z coordinates of the region’s origin are set to `0`, and the region’s height and depth are set to `1.`

## See Also

### Creating Regions

init()

Initializes a new region.

init(origin: MTLOrigin, size: MTLSize)

Initializes a new region with the specified origin and size.

func MTLRegionMake2D(Int, Int, Int, Int) -> MTLRegion

Creates a 3D representation of a 2D region.

func MTLRegionMake3D(Int, Int, Int, Int, Int, Int) -> MTLRegion

Creates a 3D region.

