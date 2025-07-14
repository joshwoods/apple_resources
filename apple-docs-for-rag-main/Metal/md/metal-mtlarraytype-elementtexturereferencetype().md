

- Metal
- MTLArrayType
-  elementTextureReferenceType() 

Instance Method

# elementTextureReferenceType()

Provides a description of the underlying texture type when an array holds textures as its elements.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func elementTextureReferenceType() -> MTLTextureReferenceType?
```

## Return Value

An object that describes the texture. If the array elements aren’t textures, this method returns `nil`.

## Discussion

Use this method if elementType is MTLDataType.texture.

## See Also

### Obtaining Details for Complex Array Elements

func element() -> MTLArrayType?

Provides a description of the underlying type when an array holds other arrays as its elements.

func elementStructType() -> MTLStructType?

Provides a description of the underlying struct type when an array holds structs as its elements.

func elementPointerType() -> MTLPointerType?

Provides a description of the underlying pointer type when an array holds pointers as its elements.

