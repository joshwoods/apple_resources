

- Metal
- MTLStructMember
-  pointerType() 

Instance Method

# pointerType()

Provides a description of the underlying pointer when the struct member holds a pointer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func pointerType() -> MTLPointerType?
```

## Return Value

An object that describes the pointer. If dataType indicates that this member isn’t a pointer, this method returns `nil`.

## See Also

### Obtaining Struct Member Details

func arrayType() -> MTLArrayType?

Provides a description of the underlying array when the struct member holds an array.

func structType() -> MTLStructType?

Provides a description of the underlying struct when the struct member holds a struct.

func textureReferenceType() -> MTLTextureReferenceType?

Provides a description of the underlying texture when the struct member holds a texture.

