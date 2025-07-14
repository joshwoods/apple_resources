

- Cinematic
- CNCustomDetectionTrack
-  init(detections:smooth:) 

Initializer

# init(detections:smooth:)

Initializes a custom detection track object with an array of detections and optionally applying smoothing.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
init(
    detections: [CNDetection],
    smooth applySmoothing: Bool
)
```

## Parameters 

`detections`  

An array of detections.

`applySmoothing`  

A flag that instructs the framework to apply a smoothing algorithm. The smoothing algorithm used, is the same that’s used for built-in detections during recording. It compensates for some amount of jitter in the disparity measure by smoothing out variability.

