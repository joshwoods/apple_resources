

- AVFoundation
- AVSpatialCaptureDiscomfortReason
-  subjectTooClose 

Type Property

# subjectTooClose

A value that indicates the focus point of the current scene is too close.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
static let subjectTooClose: AVSpatialCaptureDiscomfortReason
```

## Discussion

The playback experience would likely be uncomfortable due to the subject being closer than the minimum focus distance of one or both of the lenses.

## See Also

### Discomfort Reasons

static let notEnoughLight: AVSpatialCaptureDiscomfortReason

A value that indicates the lighting of the current scene isn’t bright enough.

