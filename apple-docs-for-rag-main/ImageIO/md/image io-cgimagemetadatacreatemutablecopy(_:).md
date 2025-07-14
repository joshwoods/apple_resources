

- Image I/O
-  CGImageMetadataCreateMutableCopy(\_:) 

Function

# CGImageMetadataCreateMutableCopy(\_:)

Creates a deep, mutable copy of the specified metadata information.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageMetadataCreateMutableCopy(_ metadata: CGImageMetadata) -> CGMutableImageMetadata?
```

## Parameters 

`metadata`  

The metadata information to copy. This function makes a deep copy of all CGImageMetadataTag structures in this parameter, including the values for the tags.

## Return Value

A new CGMutableImageMetadata type that contains a deep copy of the tags in the metadata parameter.

## Discussion

Typically, you call this function before modifying the metadata information for an image. Use it to create a copy of the image’s existing metadata information, and then add or modify that metadata before saving it with the image.

## See Also

### Creating a Mutable Metadata Type

func CGImageMetadataCreateMutable() -> CGMutableImageMetadata

Creates an empty, mutable image metdata opaque type.

