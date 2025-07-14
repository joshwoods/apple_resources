

- Metal
- MTLStructMember
-  arrayType() 

Instance Method

# arrayType()

Provides a description of the underlying array when the struct member holds an array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func arrayType() -> MTLArrayType?
```

## Return Value

An object that describes the array. If dataType indicates that this member is not an array, this method returns `nil.`

## See Also

### Obtaining Struct Member Details

func structType() -> MTLStructType?

Provides a description of the underlying struct when the struct member holds a struct.

func pointerType() -> MTLPointerType?

Provides a description of the underlying pointer when the struct member holds a pointer.

func textureReferenceType() -> MTLTextureReferenceType?

Provides a description of the underlying texture when the struct member holds a texture.

