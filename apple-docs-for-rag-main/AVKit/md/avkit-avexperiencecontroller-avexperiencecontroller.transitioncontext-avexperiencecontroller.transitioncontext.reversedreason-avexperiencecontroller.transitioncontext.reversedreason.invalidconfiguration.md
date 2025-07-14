

- AVKit
- AVExperienceController
- AVExperienceController.TransitionContext
- AVExperienceController.TransitionContext.ReversedReason
-  AVExperienceController.TransitionContext.ReversedReason.invalidConfiguration 

Case

# AVExperienceController.TransitionContext.ReversedReason.invalidConfiguration

A transition could not be completed because some required configuration was unavailable.

visionOS 2.0+

``` source
case invalidConfiguration
```

## Discussion

This can happen if AVPlayerViewController has been freed.

