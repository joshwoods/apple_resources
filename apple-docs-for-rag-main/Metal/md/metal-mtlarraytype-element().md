

- Metal
- MTLArrayType
-  element() 

Instance Method

# element()

Provides a description of the underlying type when an array holds other arrays as its elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func element() -> MTLArrayType?
```

## Return Value

Returns an object that describes an array. If the array elements aren’t arrays, this method returns `nil`.

## Discussion

Use this method if elementType is MTLDataType.array.

## See Also

### Obtaining Details for Complex Array Elements

func elementStructType() -> MTLStructType?

Provides a description of the underlying struct type when an array holds structs as its elements.

func elementPointerType() -> MTLPointerType?

Provides a description of the underlying pointer type when an array holds pointers as its elements.

func elementTextureReferenceType() -> MTLTextureReferenceType?

Provides a description of the underlying texture type when an array holds textures as its elements.

