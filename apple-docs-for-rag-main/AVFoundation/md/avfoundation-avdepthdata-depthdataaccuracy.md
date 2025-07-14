

- AVFoundation
- AVDepthData
-  depthDataAccuracy 

Instance Property

# depthDataAccuracy

The general accuracy of depth data map values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var depthDataAccuracy: AVDepthData.Accuracy { get }
```

## Discussion

The accuracy of a depth data map is highly dependent on the camera calibration data used to generate it. If the camera’s focal length cannot be precisely determined at the time of capture, a scaling error in the z (depth) plane is introduced. If the camera’s optical center can’t be precisely determined at capture time, a principal point error is introduced, leading to an offset error in the disparity estimate. AVDepthData.Accuracy constants report the accuracy of a map’s values with respect to its reported units.

## See Also

### Evaluating Depth Data

var isDepthDataFiltered: Bool

A Boolean value indicating whether the depth map contains temporally smoothed data.

enum Accuracy

Values indicating the general accuracy of a depth data map.

var depthDataQuality: AVDepthData.Quality

The overall quality of the depth map.

enum Quality

Values indicating the overall quality of a depth data map.

