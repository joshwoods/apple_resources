

- UIKit
- UIImpactFeedbackGenerator
-  impactOccurred(intensity:) 

Instance Method

# impactOccurred(intensity:)

Triggers impact feedback with a specific intensity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
func impactOccurred(intensity: CGFloat)
```

## Parameters 

`intensity`  

A CGFloat value between `0.0` and `1.0`.

## See Also

### Reporting impacts

func impactOccurred()

Triggers impact feedback.

func impactOccurred(at: CGPoint)

Triggers impact feedback at the specified location.

func impactOccurred(intensity: CGFloat, at: CGPoint)

Triggers impact feedback with a specific intensity at the specified location.

