

- AVKit
- AVExperienceController
-  AVExperienceController.Delegate 

Protocol

# AVExperienceController.Delegate

A protocol that defines the methods to implement to respond to experience changes.

visionOS 2.0+

``` source
@MainActor
protocol Delegate : AnyObject
```

## Overview

Use this delegate to be informed of transitions and to update applications state based on these changes.

## Topics

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

struct TransitionContext

The state of the transition provided to the delegate object.

## See Also

### Configuring a delegate

var delegate: (any AVExperienceController.Delegate)?

A delegate object for the experience controller.

