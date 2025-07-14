

- UIKit
- UIImpactFeedbackGenerator
-  impactOccurred() 

Instance Method

# impactOccurred()

Triggers impact feedback.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func impactOccurred()
```

## Discussion

This method tells the generator that an impact has occurred. In response, the generator may play the appropriate haptics based on the UIImpactFeedbackGenerator.FeedbackStyle value passed to the generator’s init(style:) initializer.

For information on setting up a feedback generator, see the UIFeedbackGenerator class.

## See Also

### Related Documentation

func prepare()

Prepares the generator to trigger feedback.

### Reporting impacts

func impactOccurred(intensity: CGFloat)

Triggers impact feedback with a specific intensity.

func impactOccurred(at: CGPoint)

Triggers impact feedback at the specified location.

func impactOccurred(intensity: CGFloat, at: CGPoint)

Triggers impact feedback with a specific intensity at the specified location.

