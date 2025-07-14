

- Image I/O
-  CGImageSourceCopyTypeIdentifiers() 

Function

# CGImageSourceCopyTypeIdentifiers()

Returns an array of uniform type identifiers that are supported for image sources.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceCopyTypeIdentifiers() -> CFArray
```

## Return Value

Returns an array of the uniform type identifiers that are supported for image sources.

## Discussion

For a list of system-declared and third-party identifiers, see Uniform Type Identifiers.

## See Also

### Getting Information From an Image Source

func CGImageSourceGetTypeID() -> CFTypeID

Returns the unique type identifier of an image source opaque type.

func CGImageSourceGetType(CGImageSource) -> CFString?

Returns the uniform type identifier of the source container.

func CGImageSourceGetCount(CGImageSource) -> Int

Returns the number of images (not including thumbnails) in the image source.

func CGImageSourceCopyProperties(CGImageSource, CFDictionary?) -> CFDictionary?

Returns the properties of the image source.

func CGImageSourceCopyPropertiesAtIndex(CGImageSource, Int, CFDictionary?) -> CFDictionary?

Returns the properties of the image at a specified location in an image source.

func CGImageSourceCopyAuxiliaryDataInfoAtIndex(CGImageSource, Int, CFString) -> CFDictionary?

Returns auxiliary data, such as mattes and depth information, that accompany the image.

