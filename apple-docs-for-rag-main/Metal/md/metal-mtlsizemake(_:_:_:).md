

- Metal
-  MTLSizeMake(\_:\_:\_:) 

Function

# MTLSizeMake(\_:\_:\_:)

Creates a size for an object using the specified dimensions.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func MTLSizeMake(
    _ width: Int,
    _ height: Int,
    _ depth: Int
) -> MTLSize
```

## Parameters 

`width`  

The width of the object.

`height`  

The height of the object. Set to `1` if the object only has one dimension.

`depth`  

The depth of the object. Set to `1` if the object has one or two dimensions.

## Return Value

The specified size of an object.

## See Also

### Creating Sizes

init()

Initializes a box size.

init(width: Int, height: Int, depth: Int)

Initializes a size for an object with the specified dimensions.

