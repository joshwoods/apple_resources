

- AVKit
- AVExperienceController
- AVExperienceController.Delegate
-  experienceController(\_:prepareForTransitionUsing:) 

Instance Method

# experienceController(\_:prepareForTransitionUsing:)

Tells the delegate that the system is preparing for a transition.

visionOS 2.0+

``` source
@MainActor
func experienceController(
    _ controller: AVExperienceController,
    prepareForTransitionUsing context: AVExperienceController.TransitionContext
) async
```

**Required**

## Parameters 

`controller`  

The `AVExperienceController`.

`context`  

Contains information about the transition.

## Discussion

Implement this method to prepare the app’s state for the toExperience. This may include showing or hiding view controllers, putting the player view controller in the view hierarchy, or any other asynchronous work required for the transition. This is the last chance to update configuration before the transition begins.

## See Also

### Responding to experience changes

func experienceController(AVExperienceController, didChangeAvailableExperiences: AVExperienceController.Experiences)

Tells the delegate when the available experiences change.

**Required**

func experienceController(AVExperienceController, didChangeTransitionContext: AVExperienceController.TransitionContext)

Tells the delegate when the transition context changes during a transition.

**Required**

struct TransitionContext

The state of the transition provided to the delegate object.

