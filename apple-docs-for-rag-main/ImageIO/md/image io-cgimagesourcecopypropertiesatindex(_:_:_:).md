

- Image I/O
-  CGImageSourceCopyPropertiesAtIndex(\_:\_:\_:) 

Function

# CGImageSourceCopyPropertiesAtIndex(\_:\_:\_:)

Returns the properties of the image at a specified location in an image source.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceCopyPropertiesAtIndex(
    _ isrc: CGImageSource,
    _ index: Int,
    _ options: CFDictionary?
) -> CFDictionary?
```

## Parameters 

`isrc`  

The image source that contains the image data.

`index`  

The zero-based index into the images of the image source. If the index is invalid, this method returns `NULL`.

`options`  

A dictionary you can use to request additional options. For a list of possible values, see Specifying the Read Options.

## Return Value

A dictionary that contains the properties associated with the image. See `CGImageProperties` for a list of properties that allowed in the dictionary.

## See Also

### Getting Information From an Image Source

func CGImageSourceGetTypeID() -> CFTypeID

Returns the unique type identifier of an image source opaque type.

func CGImageSourceGetType(CGImageSource) -> CFString?

Returns the uniform type identifier of the source container.

func CGImageSourceCopyTypeIdentifiers() -> CFArray

Returns an array of uniform type identifiers that are supported for image sources.

func CGImageSourceGetCount(CGImageSource) -> Int

Returns the number of images (not including thumbnails) in the image source.

func CGImageSourceCopyProperties(CGImageSource, CFDictionary?) -> CFDictionary?

Returns the properties of the image source.

func CGImageSourceCopyAuxiliaryDataInfoAtIndex(CGImageSource, Int, CFString) -> CFDictionary?

Returns auxiliary data, such as mattes and depth information, that accompany the image.

