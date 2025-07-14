

- AVKit
- AVDisplayManager
-  preferredDisplayCriteria 

Instance Property

# preferredDisplayCriteria

A hint for the TV to set the display mode to best match the currently playing content’s display criteria.

tvOS 11.2+visionOS 1.0+

``` source
@NSCopying
var preferredDisplayCriteria: AVDisplayCriteria? { get set }
```

## Discussion

The display manager uses the preferred display criteria only when user settings allow. Set this property to `nil` to allow the system to guide you to a display mode that’s suitable for a wide range of video and nonvideo content.

## See Also

### Matching a Video’s Native Display Mode

var isDisplayCriteriaMatchingEnabled: Bool

A Boolean value that indicates whether the user has enabled display critera matching.

var isDisplayModeSwitchInProgress: Bool

A Boolean value that indicates whether a display mode switch is in progress.

