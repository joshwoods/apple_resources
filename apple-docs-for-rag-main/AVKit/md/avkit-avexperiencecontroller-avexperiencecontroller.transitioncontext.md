

- AVKit
- AVExperienceController
-  AVExperienceController.TransitionContext 

Structure

# AVExperienceController.TransitionContext

The state of the transition provided to the delegate object.

visionOS 2.0+

``` source
struct TransitionContext
```

## Overview

When `AVExperienceController` transitions its `experience` from `fromExperience` to `toExperience`, delegate callbacks provide instances of `TransitionContext` to allow clients to respond as the transition progresses or reverts. The normal `Status` sequence is `.preparing` -\> `.transitioning` -\> `.completed` Once `.completed`, `AVExperienceController`’s `experience` is now the `toExperience`.

Not all transitions are `.completed`, instead they are `.reversed` back to the `fromExperience`. Reversed transitions can happen after `.preparing` or after `.transitioning`, but it will not happen after `.completed` or before `.preparing`. When a transition is reversed a reason is provided.

## Topics

### Instance Properties

let fromExperience: AVExperienceController.Experience

The experience of the `AVExperienceController` before the transition was initiated.

let status: AVExperienceController.TransitionContext.Status

The status of the transition.

let toExperience: AVExperienceController.Experience

The experience to which the `AVExperienceController` has been requested to transition to.

### Enumerations

enum ReversedReason

enum Status

Describes the status of a transition.

enum TransitionResult

Describes the result of a transition.

## Relationships

### Conforms To

- Equatable

## See Also

### Responding to experience changes

func experienceController(AVExperienceController, didChangeAvailableExperiences: AVExperienceController.Experiences)

Tells the delegate when the available experiences change.

**Required**

func experienceController(AVExperienceController, prepareForTransitionUsing: AVExperienceController.TransitionContext) async

Tells the delegate that the system is preparing for a transition.

**Required**

func experienceController(AVExperienceController, didChangeTransitionContext: AVExperienceController.TransitionContext)

Tells the delegate when the transition context changes during a transition.

**Required**

