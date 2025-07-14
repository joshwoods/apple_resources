

- AVKit
- AVExperienceController
-  AVExperienceController.Experience 

Enumeration

# AVExperienceController.Experience

The types of experiences the system supports.

visionOS 2.0+

``` source
enum Experience
```

## Topics

### Supported experiences

case embedded

An experience where the video embeds within its original container.

case expanded

An experience where the system places the video outside of its original container.

case multiview

An experience where multiple videos play together.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

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

var configuration: AVExperienceController.Configuration

The configuration options per experience.

struct Configuration

A structure that stores per-experience configuration.

