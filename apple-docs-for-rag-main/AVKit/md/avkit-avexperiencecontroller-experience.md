

- AVKit
- AVExperienceController
-  experience 

Instance Property

# experience

The current experience.

visionOS 2.0+

``` source
@MainActor
final var experience: AVExperienceController.Experience { get }
```

## Discussion

The system updates this value only after the status changes to AVExperienceController.TransitionContext.Status.finished(result:).

Implement the experienceController(_:didChangeTransitionContext:) delegate method to observe changes to this value.

## See Also

### Configuring the experience

var allowedExperiences: AVExperienceController.Experiences

The set of experiences the application supports.

var availableExperiences: AVExperienceController.Experiences

The allowed experiences that are available to use on the device at this time.

struct Experiences

A structure that represents a collection of experiences to use with an experience controller.

enum Experience

The types of experiences the system supports.

var configuration: AVExperienceController.Configuration

The configuration options per experience.

struct Configuration

A structure that stores per-experience configuration.

