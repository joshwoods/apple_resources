

- AVFoundation
-  AVSpatialCaptureDiscomfortReason 

Structure

# AVSpatialCaptureDiscomfortReason

Constants that indicate the suitability of the current scene to create a comfortable viewing experience.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
struct AVSpatialCaptureDiscomfortReason
```

## Topics

### Discomfort Reasons

static let notEnoughLight: AVSpatialCaptureDiscomfortReason

A value that indicates the lighting of the current scene isn’t bright enough.

static let subjectTooClose: AVSpatialCaptureDiscomfortReason

A value that indicates the focus point of the current scene is too close.

### Initializers

init(rawValue: String)

Creates a discomfort reason with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Spatial Capture

var spatialCaptureDiscomfortReasons: Set&lt;AVSpatialCaptureDiscomfortReason>

Reasons why current environmental conditions aren’t suitable to capturing spatial videos that are comfortable to view.

