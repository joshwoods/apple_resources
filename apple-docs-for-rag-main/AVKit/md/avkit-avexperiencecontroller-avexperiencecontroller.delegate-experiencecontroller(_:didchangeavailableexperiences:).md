

- AVKit
- AVExperienceController
- AVExperienceController.Delegate
-  experienceController(\_:didChangeAvailableExperiences:) 

Instance Method

# experienceController(\_:didChangeAvailableExperiences:)

Tells the delegate when the available experiences change.

visionOS 2.0+

``` source
@MainActor
func experienceController(
    _ controller: AVExperienceController,
    didChangeAvailableExperiences availableExperiences: AVExperienceController.Experiences
)
```

**Required**

## Parameters 

`controller`  

The experience controller.

`availableExperiences`  

The current value of availableExperiences.

## Discussion

Use this callback to hide or show interface elements based on which experiences are possible.

## See Also

### Responding to experience changes

func experienceController(AVExperienceController, prepareForTransitionUsing: AVExperienceController.TransitionContext) async

Tells the delegate that the system is preparing for a transition.

**Required**

func experienceController(AVExperienceController, didChangeTransitionContext: AVExperienceController.TransitionContext)

Tells the delegate when the transition context changes during a transition.

**Required**

struct TransitionContext

The state of the transition provided to the delegate object.

