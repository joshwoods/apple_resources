

- AVKit
- AVExperienceController
-  availableExperiences 

Instance Property

# availableExperiences

The allowed experiences that are available to use on the device at this time.

visionOS 2.0+

``` source
@MainActor
final var availableExperiences: AVExperienceController.Experiences { get }
```

## Discussion

This property is a subset of allowedExperiences, filtered for platform, device configuration, and system state.

## See Also

### Configuring the experience

var allowedExperiences: AVExperienceController.Experiences

The set of experiences the application supports.

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

