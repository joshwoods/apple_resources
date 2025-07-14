

- SwiftUI
- SensoryFeedback
-  levelChange 

Type Property

# levelChange

Indicates movement between discrete levels of pressure.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
static let levelChange: SensoryFeedback
```

## Discussion

For example, as the user presses a fast-forward button on a video player, playback could increase or decrease and haptic feedback could be provided as different levels of pressure are reached.

Only plays feedback on macOS.

## See Also

### Indicating changes and selections

static let alignment: SensoryFeedback

Indicates the alignment of a dragged item.

static let decrease: SensoryFeedback

Indicates that an important value decreased below a significant threshold.

static let increase: SensoryFeedback

Indicates that an important value increased above a significant threshold.

static let selection: SensoryFeedback

Indicates that a UI element’s values are changing.

static let pathComplete: SensoryFeedback

Indicates a drawn path has completed and/or recognized.

