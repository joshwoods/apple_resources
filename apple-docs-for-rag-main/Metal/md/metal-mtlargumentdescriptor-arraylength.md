

- Metal
- MTLArgumentDescriptor
-  arrayLength 

Instance Property

# arrayLength

The length of an array argument.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var arrayLength: Int { get set }
```

## Discussion

For a nonarray argument, this value must be `0`.

## See Also

### Setting the Descriptor’s Properties

var dataType: MTLDataType

The data type of the argument.

var index: Int

The index ID of the argument.

var access: MTLBindingAccess

The access permissions of the argument.

var constantBlockAlignment: Int

The alignment of the constant block.

var textureType: MTLTextureType

The texture type of a texture argument.

