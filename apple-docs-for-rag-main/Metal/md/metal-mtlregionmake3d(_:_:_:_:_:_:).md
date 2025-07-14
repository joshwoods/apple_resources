

- Metal
-  MTLRegionMake3D(\_:\_:\_:\_:\_:\_:) 

Function

# MTLRegionMake3D(\_:\_:\_:\_:\_:\_:)

Creates a 3D region.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func MTLRegionMake3D(
    _ x: Int,
    _ y: Int,
    _ z: Int,
    _ width: Int,
    _ height: Int,
    _ depth: Int
) -> MTLRegion
```

## Parameters 

`x`  

The x coordinate of the origin.

`y`  

The y coordinate of the origin.

`z`  

The z coordinate of the origin.

`width`  

The width of the volume.

`height`  

The height of the volume.

`depth`  

The depth of the volume.

## Return Value

A 3D region with the specified values.

## See Also

### Creating Regions

init()

Initializes a new region.

init(origin: MTLOrigin, size: MTLSize)

Initializes a new region with the specified origin and size.

func MTLRegionMake1D(Int, Int) -> MTLRegion

Creates a 3D representation of a 1D region.

func MTLRegionMake2D(Int, Int, Int, Int) -> MTLRegion

Creates a 3D representation of a 2D region.

