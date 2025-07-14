

- AVFoundation
-  AVVideoScalingModeFit 

Global Variable

# AVVideoScalingModeFit

The string identifier for scaling a video to fit the surrounding view’s dimensions.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let AVVideoScalingModeFit: String
```

## Discussion

This mode crops the video to remove the edge processing region, preserving the aspect ratio of the cropped source by reducing the specified width or height, if necessary. It doesn’t scale a small source up to larger dimensions.

## See Also

### Scaling mode

let AVVideoScalingModeKey: String

A key to retrieve the video scaling mode from a dictionary.

let AVVideoScalingModeResize: String

The string identifier for resizing a video to fit the surrounding view’s dimensions.

let AVVideoScalingModeResizeAspect: String

The string identifier for resizing a video to its surrounding view’s shorter dimension while preserving its aspect ratio.

let AVVideoScalingModeResizeAspectFill: String

The string identifier for resizing a video to fit the surrounding view’s longer dimension while preserving aspect ratio.

