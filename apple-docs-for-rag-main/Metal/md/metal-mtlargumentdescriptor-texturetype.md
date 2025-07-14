

- Metal
- MTLArgumentDescriptor
-  textureType 

Instance Property

# textureType

The texture type of a texture argument.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var textureType: MTLTextureType { get set }
```

## Discussion

For a nontexture argument, this value is ignored.

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

var constantBlockAlignment: Int

The alignment of the constant block.

