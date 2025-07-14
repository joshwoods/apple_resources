

- AVKit
- AVExperienceController
-  allowedExperiences 

Instance Property

# allowedExperiences

The set of experiences the application supports.

visionOS 2.0+

``` source
@MainActor
final var allowedExperiences: AVExperienceController.Experiences { get set }
```

## Discussion

Use this to allow additional experiences like multiview, or to disable expanded. This list is the basis for availableExperiences, which filters out inapplicable experiences.

Note

Because AVExperienceController.Experience.embedded is the initial experience, and the one returned to when others end, it’s a programming error to exclude it from this list.

## See Also

### Configuring the experience

var availableExperiences: AVExperienceController.Experiences

The allowed experiences that are available to use on the device at this time.

struct Experiences

A structure that represents a collection of experiences to use with an experience controller.

var experience: AVExperienceController.Experience

The current experience.

enum Experience

The types of experiences the system supports.

var configuration: AVExperienceController.Configuration

The configuration options per experience.

struct Configuration

A structure that stores per-experience configuration.

