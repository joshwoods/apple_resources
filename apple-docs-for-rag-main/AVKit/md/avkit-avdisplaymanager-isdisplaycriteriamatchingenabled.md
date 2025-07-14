

- AVKit
- AVDisplayManager
-  isDisplayCriteriaMatchingEnabled 

Instance Property

# isDisplayCriteriaMatchingEnabled

A Boolean value that indicates whether the user has enabled display critera matching.

tvOS 11.3+visionOS 1.0+

``` source
var isDisplayCriteriaMatchingEnabled: Bool { get }
```

## Discussion

This value reflects the user’s current Match Content settings, which they set in the Settings app under Video and Audio \> Match Content.

## See Also

### Matching a Video’s Native Display Mode

var preferredDisplayCriteria: AVDisplayCriteria?

A hint for the TV to set the display mode to best match the currently playing content’s display criteria.

var isDisplayModeSwitchInProgress: Bool

A Boolean value that indicates whether a display mode switch is in progress.

