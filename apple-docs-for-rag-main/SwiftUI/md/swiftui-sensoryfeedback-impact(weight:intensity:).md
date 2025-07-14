

- SwiftUI
- SensoryFeedback
-  impact(weight:intensity:) 

Type Method

# impact(weight:intensity:)

Provides a physical metaphor you can use to complement a visual experience.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
static func impact(
    weight: SensoryFeedback.Weight = .medium,
    intensity: Double = 1.0
) -> SensoryFeedback
```

## Discussion

Use this to provide feedback for UI elements colliding. It should supplement the user experience, since only some platforms will play feedback in response to it.

Not all platforms will play different feedback for different weights and intensities of impact.

Only plays feedback on iOS and watchOS.

## See Also

### Producing a physical impact

static let impact: SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

static func impact(flexibility: SensoryFeedback.Flexibility, intensity: Double) -> SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

struct Flexibility

The flexibility to be represented by a type of feedback.

struct Weight

The weight to be represented by a type of feedback.

