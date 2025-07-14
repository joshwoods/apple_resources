

- AVFoundation
- AVDepthData
-  isDepthDataFiltered 

Instance Property

# isDepthDataFiltered

A Boolean value indicating whether the depth map contains temporally smoothed data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var isDepthDataFiltered: Bool { get }
```

## Discussion

The capture system can smooth noise and fill in missing values (caused by low light or lens occlusion) in depth data maps by temporally interpolating between previous and subsequent frames of captured depth data. Use the AVCaptureDepthDataOutput isFilteringEnabled property to control filtering for streaming depth capture, or the AVCapturePhotoSettings isDepthDataFiltered property to control filtering for depth data captured alongside photo capture.

Filtering depth data makes it more useful for applying visual effects to a companion image, but alters the data such that it may no longer be suitable for computer vision tasks. (In an unfiltered depth map, missing values are represented as `NaN`.)

## See Also

### Evaluating Depth Data

var depthDataAccuracy: AVDepthData.Accuracy

The general accuracy of depth data map values.

enum Accuracy

Values indicating the general accuracy of a depth data map.

var depthDataQuality: AVDepthData.Quality

The overall quality of the depth map.

enum Quality

Values indicating the overall quality of a depth data map.

