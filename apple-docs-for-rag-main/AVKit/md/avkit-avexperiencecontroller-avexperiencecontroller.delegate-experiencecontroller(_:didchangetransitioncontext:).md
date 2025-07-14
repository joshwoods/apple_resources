

- AVKit
- AVExperienceController
- AVExperienceController.Delegate
-  experienceController(\_:didChangeTransitionContext:) 

Instance Method

# experienceController(\_:didChangeTransitionContext:)

Tells the delegate when the transition context changes during a transition.

visionOS 2.0+

``` source
@MainActor
func experienceController(
    _ controller: AVExperienceController,
    didChangeTransitionContext context: AVExperienceController.TransitionContext
)
```

**Required**

## Parameters 

`controller`  

The experience controller.

`context`  

An structure that contains information about the transition.

## Discussion

Implement this method to track the transition between experiences.

## See Also

### Responding to experience changes

func experienceController(AVExperienceController, didChangeAvailableExperiences: AVExperienceController.Experiences)

Tells the delegate when the available experiences change.

**Required**

func experienceController(AVExperienceController, prepareForTransitionUsing: AVExperienceController.TransitionContext) async

Tells the delegate that the system is preparing for a transition.

**Required**

struct TransitionContext

The state of the transition provided to the delegate object.

