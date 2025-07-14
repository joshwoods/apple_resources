

- AVKit
- AVExperienceController
- AVExperienceController.ExpandedConfiguration
-  fallbackPlacement 

Instance Property

# fallbackPlacement

A fallback placement to use when the original container isn’t in the view controller hierarchy.

visionOS 2.0+

``` source
var fallbackPlacement: AVExperienceController.ExpandedConfiguration.Placement
```

## Discussion

The system places expanded experience over the scene of the original container. When the container isn’t available, the system uses this value. If neither specifies a valid placement, attempting to transition to an expanded experience fails.

## See Also

### Specifying placement

struct Placement

A structure that represents where the video will be experienced.

