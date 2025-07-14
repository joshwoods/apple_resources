

- SwiftUI
- SensoryFeedback
-  SensoryFeedback.Weight 

Structure

# SensoryFeedback.Weight

The weight to be represented by a type of feedback.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
struct Weight
```

## Overview

`Weight` values can be passed to `SensoryFeedback.impact(weight:intensity:)`.

## Topics

### Getting flexibility values

static let light: SensoryFeedback.Weight

Indicates a collision between small or lightweight UI objects.

static let medium: SensoryFeedback.Weight

Indicates a collision between medium-sized or medium-weight UI objects.

static let heavy: SensoryFeedback.Weight

Indicates a collision between large or heavyweight UI objects.

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

struct Flexibility

The flexibility to be represented by a type of feedback.

