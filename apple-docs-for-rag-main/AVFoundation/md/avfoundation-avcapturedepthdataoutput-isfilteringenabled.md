

- AVFoundation
- AVCaptureDepthDataOutput
-  isFilteringEnabled 

Instance Property

# isFilteringEnabled

A Boolean value that determines whether the depth data output should filter depth data to smooth out noise and fill invalid values.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isFilteringEnabled: Bool { get set }
```

## Discussion

When this value is true (the default), the capture output smooths noise and fills in missing or invalid values (caused by low light or lens occlusion) in depth data maps by temporally interpolating between previous and subsequent frames of captured depth data.

Filtering depth data makes it more useful for applying visual effects to a companion image, but alters the data such that it may no longer be suitable for computer vision tasks. (In an unfiltered depth map, missing values are represented as `NaN`.)

## See Also

### Configuring Depth Data Capture

var alwaysDiscardsLateDepthData: Bool

A Boolean value that determines whether the capture output should discard any depth data that is not processed before the next depth data is captured.

