

- Cinematic
- CNObjectTracker
-  startTracking(at:within:sourceImage:sourceDisparity:) 

Instance Method

# startTracking(at:within:sourceImage:sourceDisparity:)

Starts creating a detection track to track an object within the given bounds.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
func startTracking(
    at time: CMTime,
    within normalizedBounds: CGRect,
    sourceImage: CVPixelBuffer,
    sourceDisparity: CVPixelBuffer
) -> Bool
```

## Parameters 

`time`  

The presentation time of the first frame in the detection track.

`normalizedBounds`  

The bounds of the object to track in normalized coordinates where (0.0, 0.0) is the upper-left corner, and (1.0, 1.0) is the lower-right.

`sourceImage`  

The image buffer containing the image.

`sourceDisparity`  

The disparity buffer containing depth information.

## Return Value

A flag representing whether the object can be tracked.

## Discussion

If you can track the object, the system adds a detection to the detection track you’re building.

