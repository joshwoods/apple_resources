

- Metal
- MTLArgumentDescriptor
-  dataType 

Instance Property

# dataType

The data type of the argument.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var dataType: MTLDataType { get set }
```

## Discussion

For a constant data argument, this value must match the binary format of the data stored in the buffer for that argument. For other parameter types, such as textures or samplers, specify the appropriate constant. See MTLDataType for possible values.

## See Also

### Setting the Descriptor’s Properties

var index: Int

The index ID of the argument.

var access: MTLBindingAccess

The access permissions of the argument.

var arrayLength: Int

The length of an array argument.

var constantBlockAlignment: Int

The alignment of the constant block.

var textureType: MTLTextureType

The texture type of a texture argument.

