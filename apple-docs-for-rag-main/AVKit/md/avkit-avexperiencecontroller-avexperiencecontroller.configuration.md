

- AVKit
- AVExperienceController
-  AVExperienceController.Configuration 

Structure

# AVExperienceController.Configuration

A structure that stores per-experience configuration.

visionOS 2.0+

``` source
struct Configuration
```

## Topics

### Configuring experiences

var expanded: AVExperienceController.ExpandedConfiguration

Configuration options for an expanded experience.

struct ExpandedConfiguration

A structure that specifies options for an expanded experience.

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

var configuration: AVExperienceController.Configuration

The configuration options per experience.

