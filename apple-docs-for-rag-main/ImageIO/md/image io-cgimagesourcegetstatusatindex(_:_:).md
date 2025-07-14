

- Image I/O
-  CGImageSourceGetStatusAtIndex(\_:\_:) 

Function

# CGImageSourceGetStatusAtIndex(\_:\_:)

Returns the current status of an image at the specified location in the image source.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceGetStatusAtIndex(
    _ isrc: CGImageSource,
    _ index: Int
) -> CGImageSourceStatus
```

## Parameters 

`isrc`  

The image source that contains the image data.

`index`  

The zero-based index into the images of the image source. If the index is invalid, this method returns `NULL`.

## Return Value

Returns the current status of the image. See CGImageSourceStatus for a list of possible values.

## Discussion

Status information is particularly informative for incremental image sources, but you may also use it on image sources that contain non-incremental data.

## See Also

### Getting the Image Status

func CGImageSourceGetStatus(CGImageSource) -> CGImageSourceStatus

Return the status of an image source.

enum CGImageSourceStatus

The set of status values for images and image sources.

