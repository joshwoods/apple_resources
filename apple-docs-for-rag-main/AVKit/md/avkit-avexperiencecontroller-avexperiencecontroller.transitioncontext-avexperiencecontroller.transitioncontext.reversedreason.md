

- AVKit
- AVExperienceController
- AVExperienceController.TransitionContext
-  AVExperienceController.TransitionContext.ReversedReason 

Enumeration

# AVExperienceController.TransitionContext.ReversedReason

visionOS 2.0+

``` source
enum ReversedReason
```

## Topics

### Enumeration Cases

case invalidConfiguration

A transition could not be completed because some required configuration was unavailable.

case invalidExperience

A transition was attempted with an experience that cannot be transitioned to.

case transitionCancelled

A transition in progress has been cancelled.

case transitionFailed

A transition has failed.

case transitionInProgress

A transition was attempted while another transition was in progress.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

