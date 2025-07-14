

- Cinematic
- CNObjectTracker
-  continueTracking(at:sourceImage:sourceDisparity:) 

Instance Method

# continueTracking(at:sourceImage:sourceDisparity:)

An object that continues to track an object that you’ve started tracking, and adds a new detection to the detection track you’re building.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
func continueTracking(
    at time: CMTime,
    sourceImage: CVPixelBuffer,
    sourceDisparity: CVPixelBuffer
) -> CNBoundsPrediction?
```

## Parameters 

`time`  

The presentation time of the first frame in the detection track.

`sourceImage`  

The image buffer containing the image.

`sourceDisparity`  

The disparity buffer containing depth information.

## Return Value

An object representing a prediction of where the object is in the source image.

