

- UIKit
- UIImpactFeedbackGenerator
-  impactOccurred(intensity:at:) 

Instance Method

# impactOccurred(intensity:at:)

Triggers impact feedback with a specific intensity at the specified location.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
func impactOccurred(
    intensity: CGFloat,
    at location: CGPoint
)
```

## See Also

### Reporting impacts

func impactOccurred()

Triggers impact feedback.

func impactOccurred(intensity: CGFloat)

Triggers impact feedback with a specific intensity.

func impactOccurred(at: CGPoint)

Triggers impact feedback at the specified location.

