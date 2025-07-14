

- Metal
- MTLMapIndirectArguments
-  init(regionOriginX:regionOriginY:regionOriginZ:regionSizeWidth:regionSizeHeight:regionSizeDepth:mipMapLevel:sliceId:) 

Initializer

# init(regionOriginX:regionOriginY:regionOriginZ:regionSizeWidth:regionSizeHeight:regionSizeDepth:mipMapLevel:sliceId:)

Returns a new data layout for mapping sparse texture regions.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    regionOriginX: UInt32,
    regionOriginY: UInt32,
    regionOriginZ: UInt32,
    regionSizeWidth: UInt32,
    regionSizeHeight: UInt32,
    regionSizeDepth: UInt32,
    mipMapLevel: UInt32,
    sliceId: UInt32
)
```

## Parameters 

`regionOriginX`  

The x coordinate of the region to change, measured in tile coordinates.

`regionOriginY`  

The y coordinate of the region to change, measured in tile coordinates.

`regionOriginZ`  

The z coordinate of the region to change, measured in tile coordinates.

`regionSizeWidth`  

The width of the region, measured in tile coordinates.

`regionSizeHeight`  

The height of the region, measured in tile coordinates.

`regionSizeDepth`  

The depth of the region, measured in tile coordinates.

`mipMapLevel`  

The mipmap to change.

`sliceId`  

The texture slice to change.

## See Also

### Creating Indirect Mapping Arguments

init()

Returns a default data layout for mapping sparse texture regions.

