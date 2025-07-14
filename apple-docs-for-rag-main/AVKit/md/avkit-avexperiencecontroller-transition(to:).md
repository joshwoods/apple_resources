

- AVKit
- AVExperienceController
-  transition(to:) 

Instance Method

# transition(to:)

Transitions the video to a different experience.

visionOS 2.0+

``` source
@discardableResult @MainActor
final func transition(to toExperience: AVExperienceController.Experience) async -> AVExperienceController.TransitionContext.TransitionResult
```

## Parameters 

`toExperience`  

The experience to transition to.

## Return Value

A transition result.

## Discussion

Call this method to transition to a different experience such as AVExperienceController.Experience.expanded. When you initiate a transition, the system calls the experience controller’s delegate methods so your app can respond to experience changes.

You determine the success of a transition by evaluating the AVExperienceController.TransitionContext.TransitionResult this method returns. A transition result of AVExperienceController.TransitionContext.TransitionResult.completed indicates a successful transition, in which case the system updates the experience property to the new experience. A transition result of AVExperienceController.TransitionContext.TransitionResult.reversed(reason:) indicates a failed transition. Evaluate the the result’s AVExperienceController.TransitionContext.ReversedReason to determine why the transition failed. A failure that occurs before the transition begins results in the system not invoking any delegate callback methods. If the failure happens after the callback to experienceController(_:prepareForTransitionUsing:) occurs, the transition context changes to AVExperienceController.TransitionContext.Status.finished(result:).

