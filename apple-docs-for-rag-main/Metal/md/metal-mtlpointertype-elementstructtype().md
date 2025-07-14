

- Metal
- MTLPointerType
-  elementStructType() 

Instance Method

# elementStructType()

Provides a description of the underlying struct when the pointer points to a struct.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func elementStructType() -> MTLStructType?
```

## Return Value

An object that describes the struct. If the pointer does not point to an struct, this method returns `nil`.

## See Also

### Obtaining Details for Complex Pointer Elements

func elementArrayType() -> MTLArrayType?

Provides a description of the underlying array when the pointer points to an array.

