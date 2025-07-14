

- AVKit
- AVExperienceController
- AVExperienceController.TransitionContext
-  AVExperienceController.TransitionContext.Status 

Enumeration

# AVExperienceController.TransitionContext.Status

Describes the status of a transition.

visionOS 2.0+

``` source
enum Status
```

## Overview

Transitions go through a sequence of `Status`s as they progress.

## Topics

### Enumeration Cases

case finished(result: AVExperienceController.TransitionContext.TransitionResult)

Transition finished. Perform cleanup based on result.

case preparing

The transition is preparing for `toExperience`.

case transitioning

The transition is in progress.

## Relationships

### Conforms To

- Equatable

