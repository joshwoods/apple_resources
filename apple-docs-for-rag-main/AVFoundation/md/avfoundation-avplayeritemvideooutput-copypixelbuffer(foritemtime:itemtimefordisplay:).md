

- AVFoundation
- AVPlayerItemVideoOutput
-  copyPixelBuffer(forItemTime:itemTimeForDisplay:) 

Instance Method

# copyPixelBuffer(forItemTime:itemTimeForDisplay:)

Retrieves an image that is appropriate for display at the specified item time, and marks the image as acquired.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func copyPixelBuffer(
    forItemTime itemTime: CMTime,
    itemTimeForDisplay outItemTimeForDisplay: UnsafeMutablePointer?
) -> CVPixelBuffer?
```

## Parameters 

`itemTime`  

The time at which you want to retrieve the image from the item.

`outItemTimeForDisplay`  

The time by which you intend to use the returned pixel buffer. You may specify `nil` for this parameter if you do not have a specific deadline.

## Return Value

A pixel buffer containing the image data to display or `nil` if nothing should be displayed at the specified time. The caller is responsible for calling CVBufferRelease on the returned data when it is no longer needed.

## Discussion

Typically, you call this method in response to a CVDisplayLink callback or a CADisplayLink delegate method call when the hasNewPixelBuffer(forItemTime:) method also returns true.

After calling this method, the video output object marks the pixel buffer data as having been acquired. This causes the hasNewPixelBuffer(forItemTime:) method to return false unless newer data becomes available.

## See Also

### Getting Pixel Buffer Data

func hasNewPixelBuffer(forItemTime: CMTime) -> Bool

Returns a Boolean value that indicates whether video output is available for the specified item time.

