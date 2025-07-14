

- AVFoundation
- AVPlayerItemVideoOutput
-  hasNewPixelBuffer(forItemTime:) 

Instance Method

# hasNewPixelBuffer(forItemTime:)

Returns a Boolean value that indicates whether video output is available for the specified item time.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func hasNewPixelBuffer(forItemTime itemTime: CMTime) -> Bool
```

## Parameters 

`itemTime`  

The item time to query. The time value is relative to the AVPlayerItem object with which the receiver is associated.

## Return Value

true if there is available video output that has not been previously acquired or false if there is not.

## Discussion

This method returns true if the video data at the specified time has not yet been acquired or is different from the video that was acquired previously. If you require multiple objects to acquire video output from the same AVPlayerItem object, you should create separate `AVPlayerItemVideoOutput` objects for each.

## See Also

### Getting Pixel Buffer Data

func copyPixelBuffer(forItemTime: CMTime, itemTimeForDisplay: UnsafeMutablePointer&lt;CMTime>?) -> CVPixelBuffer?

Retrieves an image that is appropriate for display at the specified item time, and marks the image as acquired.

