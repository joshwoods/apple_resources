

- Metal
- MTLStructMember
-  structType() 

Instance Method

# structType()

Provides a description of the underlying struct when the struct member holds a struct.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func structType() -> MTLStructType?
```

## Return Value

An object that describes the struct. If dataType indicates that this member is not a struct, this method returns `nil`.

## See Also

### Obtaining Struct Member Details

func arrayType() -> MTLArrayType?

Provides a description of the underlying array when the struct member holds an array.

func pointerType() -> MTLPointerType?

Provides a description of the underlying pointer when the struct member holds a pointer.

func textureReferenceType() -> MTLTextureReferenceType?

Provides a description of the underlying texture when the struct member holds a texture.

