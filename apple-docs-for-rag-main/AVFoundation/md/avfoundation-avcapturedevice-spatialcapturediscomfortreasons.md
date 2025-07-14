

- AVFoundation
- AVCaptureDevice
-  spatialCaptureDiscomfortReasons 

Instance Property

# spatialCaptureDiscomfortReasons

Reasons why current environmental conditions aren’t suitable to capturing spatial videos that are comfortable to view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var spatialCaptureDiscomfortReasons: Set { get }
```

## Discussion

You can monitor this property to determine whether to present UI that recommends a person reframe their scene for more pleasing spatial capture. For example, you could show a message that indicates the subject is too close or the scene is too dark.

## See Also

### Supporting Spatial Capture

struct AVSpatialCaptureDiscomfortReason

Constants that indicate the suitability of the current scene to create a comfortable viewing experience.

