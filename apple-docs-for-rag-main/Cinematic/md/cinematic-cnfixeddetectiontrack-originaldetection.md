

- Cinematic
- CNFixedDetectionTrack
-  originalDetection 

Instance Property

# originalDetection

The original detection based on the fixed detection track.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
var originalDetection: CNDetection? { get }
```

## Discussion

This is the way to determine the time and bounds from which the fixed focus originated. This detection isn’t part of the detection track and has a different detection ID or none.

Important

To get a detection from the fixed detection track, use detectionAtOrBeforeTime: instead, which returns a properly time-stamped detection.

