

- AVKit
- AVExperienceController
-  AVExperienceController.ExpandedConfiguration 

Structure

# AVExperienceController.ExpandedConfiguration

A structure that specifies options for an expanded experience.

visionOS 2.0+

``` source
struct ExpandedConfiguration
```

## Overview

It’s valid to transition to this experience even when the original container isn’t in a view hierarchy. In this case, you must specify a fallbackPlacement or the transition result is AVExperienceController.TransitionContext.TransitionResult.reversed(reason:).

## Topics

### Creating an expanded configuration

init(fallbackPlacement: AVExperienceController.ExpandedConfiguration.Placement)

Creates a configuration object for an expanded experience.

### Specifying placement

var fallbackPlacement: AVExperienceController.ExpandedConfiguration.Placement

A fallback placement to use when the original container isn’t in the view controller hierarchy.

struct Placement

A structure that represents where the video will be experienced.

## See Also

### Configuring experiences

var expanded: AVExperienceController.ExpandedConfiguration

Configuration options for an expanded experience.

