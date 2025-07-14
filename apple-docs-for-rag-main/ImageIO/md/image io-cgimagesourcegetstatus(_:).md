

- Image I/O
-  CGImageSourceGetStatus(\_:) 

Function

# CGImageSourceGetStatus(\_:)

Return the status of an image source.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageSourceGetStatus(_ isrc: CGImageSource) -> CGImageSourceStatus
```

## Parameters 

`isrc`  

The image source that contains the image data.

## Return Value

Returns the current status of the image source. See CGImageSourceStatus for a list of possible values.

## Discussion

Status information is particularly informative for incremental image sources, but it may also be useful on image sources that contain non-incremental data.

## See Also

### Getting the Image Status

func CGImageSourceGetStatusAtIndex(CGImageSource, Int) -> CGImageSourceStatus

Returns the current status of an image at the specified location in the image source.

enum CGImageSourceStatus

The set of status values for images and image sources.

