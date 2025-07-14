

- Image I/O
-  CGImageMetadataCreateMutable() 

Function

# CGImageMetadataCreateMutable()

Creates an empty, mutable image metdata opaque type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataCreateMutable() -> CGMutableImageMetadata
```

## Return Value

A CGMutableImageMetadata object that contains no metadata information, or `NULL` if an error occurs. You are responsible for releasing the returned object.

## See Also

### Creating a Mutable Metadata Type

func CGImageMetadataCreateMutableCopy(CGImageMetadata) -> CGMutableImageMetadata?

Creates a deep, mutable copy of the specified metadata information.

