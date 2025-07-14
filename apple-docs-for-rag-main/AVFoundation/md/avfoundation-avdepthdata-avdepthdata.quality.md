

- AVFoundation
- AVDepthData
-  AVDepthData.Quality 

Enumeration

# AVDepthData.Quality

Values indicating the overall quality of a depth data map.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum Quality
```

## Topics

### Depth Quality Values

case low

The depth map is a poor candidate for rendering high-quality depth effects or reconstructing a 3D scene.

case high

The depth map is a good candidate for rendering high-quality depth effects or reconstructing a 3D scene.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Evaluating Depth Data

var isDepthDataFiltered: Bool

A Boolean value indicating whether the depth map contains temporally smoothed data.

var depthDataAccuracy: AVDepthData.Accuracy

The general accuracy of depth data map values.

enum Accuracy

Values indicating the general accuracy of a depth data map.

var depthDataQuality: AVDepthData.Quality

The overall quality of the depth map.

