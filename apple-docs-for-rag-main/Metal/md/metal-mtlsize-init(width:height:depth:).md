

- Metal
- MTLSize
-  init(width:height:depth:) 

Initializer

# init(width:height:depth:)

Initializes a size for an object with the specified dimensions.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    width: Int,
    height: Int,
    depth: Int
)
```

## Parameters 

`width`  

The width of the volume.

`height`  

The height of the volume. Set to `1` if the object only has one dimension.

`depth`  

The depth of the volume. Set to 1 if the object has one or two dimensions.

## See Also

### Creating Sizes

init()

Initializes a box size.

func MTLSizeMake(Int, Int, Int) -> MTLSize

Creates a size for an object using the specified dimensions.

