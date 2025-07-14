

- Cinematic
- CNDetectionTrack
-  isDiscrete 

Instance Property

# isDiscrete

A flag determining if the detection track has discrete detections, otherwise continuous.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
var isDiscrete: Bool { get }
```

## Discussion

A discrete detection track returns detections only at the specific times a detection occurs. A continuous detection track returns a detection for any requested time and an empty array for time ranges.

