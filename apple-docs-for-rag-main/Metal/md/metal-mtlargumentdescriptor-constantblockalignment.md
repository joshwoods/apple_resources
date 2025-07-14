

- Metal
- MTLArgumentDescriptor
-  constantBlockAlignment 

Instance Property

# constantBlockAlignment

The alignment of the constant block.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var constantBlockAlignment: Int { get set }
```

## Discussion

If set, this property forces the constant block to be aligned to the specified value. It should be set on the first constant only, and is valid only if a corresponding explicit `alignas` specifier is applied to the constant in the Metal shader language.

## See Also

### Setting the Descriptor’s Properties

var dataType: MTLDataType

The data type of the argument.

var index: Int

The index ID of the argument.

var access: MTLBindingAccess

The access permissions of the argument.

var arrayLength: Int

The length of an array argument.

var textureType: MTLTextureType

The texture type of a texture argument.

