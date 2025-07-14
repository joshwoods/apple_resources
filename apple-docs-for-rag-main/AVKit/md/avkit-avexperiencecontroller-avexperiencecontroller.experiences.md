

- AVKit
- AVExperienceController
-  AVExperienceController.Experiences 

Structure

# AVExperienceController.Experiences

A structure that represents a collection of experiences to use with an experience controller.

visionOS 2.0+

``` source
struct Experiences
```

## Overview

When creating, choose between using only(_:) or recommended(excluding:including:). Use only(_:) to specify the list of supported experiences. Use recommended(excluding:including:) to include the default set of experiences appropriate for a given platform.

Experiences can be explicitly included or excluded from this list with the corresponding parameters.

## Topics

### Defining experiences

static func only&lt;C>(C) -> AVExperienceController.Experiences

Returns a set of experiences for the provided list.

static func recommended&lt;C>(excluding: C, including: C) -> AVExperienceController.Experiences

Returns the recommended set of experiences.

## Relationships

### Conforms To

- Collection
- Sequence

## See Also

### Configuring the experience

var allowedExperiences: AVExperienceController.Experiences

The set of experiences the application supports.

var availableExperiences: AVExperienceController.Experiences

The allowed experiences that are available to use on the device at this time.

var experience: AVExperienceController.Experience

The current experience.

enum Experience

The types of experiences the system supports.

var configuration: AVExperienceController.Configuration

The configuration options per experience.

struct Configuration

A structure that stores per-experience configuration.

