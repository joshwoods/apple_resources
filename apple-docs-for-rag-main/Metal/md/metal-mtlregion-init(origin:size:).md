

- Metal
- MTLRegion
-  init(origin:size:) 

Initializer

# init(origin:size:)

Initializes a new region with the specified origin and size.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    origin: MTLOrigin,
    size: MTLSize
)
```

## Parameters 

`origin`  

The origin of the region.

`size`  

The size of the region.

## See Also

### Creating Regions

init()

Initializes a new region.

func MTLRegionMake1D(Int, Int) -> MTLRegion

Creates a 3D representation of a 1D region.

func MTLRegionMake2D(Int, Int, Int, Int) -> MTLRegion

Creates a 3D representation of a 2D region.

func MTLRegionMake3D(Int, Int, Int, Int, Int, Int) -> MTLRegion

Creates a 3D region.

