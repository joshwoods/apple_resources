

- AVKit
- AVExperienceController
-  configuration 

Instance Property

# configuration

The configuration options per experience.

visionOS 2.0+

``` source
@MainActor
final var configuration: AVExperienceController.Configuration
```

## Discussion

You may modify the configuration at any time, but after the experienceController(_:prepareForTransitionUsing:) delegate callback returns, the system copies the configuration and uses it for the ensuing transition. Further modifications affect subsequent transitions.

## See Also

### Configuring the experience

var allowedExperiences: AVExperienceController.Experiences

The set of experiences the application supports.

var availableExperiences: AVExperienceController.Experiences

The allowed experiences that are available to use on the device at this time.

struct Experiences

A structure that represents a collection of experiences to use with an experience controller.

var experience: AVExperienceController.Experience

The current experience.

enum Experience

The types of experiences the system supports.

struct Configuration

A structure that stores per-experience configuration.

