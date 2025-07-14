

- AVKit
- AVExperienceController
- AVExperienceController.TransitionContext
- AVExperienceController.TransitionContext.ReversedReason
-  AVExperienceController.TransitionContext.ReversedReason.invalidExperience 

Case

# AVExperienceController.TransitionContext.ReversedReason.invalidExperience

A transition was attempted with an experience that cannot be transitioned to.

visionOS 2.0+

``` source
case invalidExperience
```

## Discussion

Possible response is to consult `AVExperienceController.experience` and `AVExperienceController.availableExperiences` to choose a different experience to transition to.

