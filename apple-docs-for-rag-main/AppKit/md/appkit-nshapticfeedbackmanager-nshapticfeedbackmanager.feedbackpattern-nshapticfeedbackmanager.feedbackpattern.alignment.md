

- AppKit
- NSHapticFeedbackManager
- NSHapticFeedbackManager.FeedbackPattern
-  NSHapticFeedbackManager.FeedbackPattern.alignment 

Case

# NSHapticFeedbackManager.FeedbackPattern.alignment

A haptic feedback pattern to be used in response to the alignment of an object the user is dragging around. For example, this pattern of feedback could be used in a drawing app when the user drags a shape into alignment with another shape. Other scenarios where this type of feedback could be used might include scaling an object to fit within specific dimensions, positioning an object at a preferred location, or reaching the beginning/minimum or end/maximum of something, such as a track view in an audio/video app.

macOS 10.11+

``` source
case alignment
```

## See Also

### Constants

case generic

A general haptic feedback pattern. Use this when no other feedback patterns apply.

case levelChange

A haptic feedback pattern to be used as the user moves between discrete levels of pressure. This pattern of feedback is used by multilevel accelerator buttons (class NSMultiLevelAcceleratorButton).

