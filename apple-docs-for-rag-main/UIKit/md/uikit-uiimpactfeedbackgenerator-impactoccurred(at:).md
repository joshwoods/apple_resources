

- UIKit
- UIImpactFeedbackGenerator
-  impactOccurred(at:) 

Instance Method

# impactOccurred(at:)

Triggers impact feedback at the specified location.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+

``` source
@MainActor
func impactOccurred(at location: CGPoint)
```

## See Also

### Reporting impacts

func impactOccurred()

Triggers impact feedback.

func impactOccurred(intensity: CGFloat)

Triggers impact feedback with a specific intensity.

func impactOccurred(intensity: CGFloat, at: CGPoint)

Triggers impact feedback with a specific intensity at the specified location.

