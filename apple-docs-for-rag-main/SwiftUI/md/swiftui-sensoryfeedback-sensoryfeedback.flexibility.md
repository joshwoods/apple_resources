

- SwiftUI
- SensoryFeedback
-  SensoryFeedback.Flexibility 

Structure

# SensoryFeedback.Flexibility

The flexibility to be represented by a type of feedback.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
struct Flexibility
```

## Overview

`Flexibility` values can be passed to `SensoryFeedback.impact(flexibility:intensity:)`.

## Topics

### Getting flexibility values

static let rigid: SensoryFeedback.Flexibility

Indicates a collision between hard or inflexible UI objects.

static let soft: SensoryFeedback.Flexibility

Indicates a collision between soft or flexible UI objects.

static let solid: SensoryFeedback.Flexibility

Indicates a collision between solid UI objects of medium flexibility.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Producing a physical impact

static let impact: SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

static func impact(weight: SensoryFeedback.Weight, intensity: Double) -> SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

static func impact(flexibility: SensoryFeedback.Flexibility, intensity: Double) -> SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

struct Weight

The weight to be represented by a type of feedback.

