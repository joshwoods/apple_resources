

- Image I/O
-  CGImageSourceCopyAuxiliaryDataInfoAtIndex(\_:\_:\_:) 

Function

# CGImageSourceCopyAuxiliaryDataInfoAtIndex(\_:\_:\_:)

Returns auxiliary data, such as mattes and depth information, that accompany the image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func CGImageSourceCopyAuxiliaryDataInfoAtIndex(
    _ isrc: CGImageSource,
    _ index: Int,
    _ auxiliaryImageDataType: CFString
) -> CFDictionary?
```

## Parameters 

`isrc`  

The image source that contains the image data.

`index`  

The zero-based index into the images of the image source. If the index is invalid, this method returns `NULL`.

`auxiliaryImageDataType`  

The auxiliary data to retrieve. For a list of possible values, see Auxiliary Image Data and Auxiliary Data Types.

## Return Value

A dictionary that contains the auxiliary data, or `NULL` if an error occurs.

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

func CGImageSourceCopyPropertiesAtIndex(CGImageSource, Int, CFDictionary?) -> CFDictionary?

Returns the properties of the image at a specified location in an image source.

