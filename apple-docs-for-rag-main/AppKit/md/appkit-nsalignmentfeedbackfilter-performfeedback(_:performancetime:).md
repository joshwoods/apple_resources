

- AppKit
- NSAlignmentFeedbackFilter
-  performFeedback(\_:performanceTime:) 

Instance Method

# performFeedback(\_:performanceTime:)

Performs the haptic feedback described by one or more alignment feedback tokens.

macOS 10.11+

``` source
func performFeedback(
    _ alignmentFeedbackTokens: [any NSAlignmentFeedbackToken],
    performanceTime: NSHapticFeedbackManager.PerformanceTime
)
```

## Parameters 

`alignmentFeedbackTokens`  

One or more feedback tokens prepared for specific alignment locations by calling alignmentFeedbackTokenForMovement(in:previousPoint:alignedPoint:defaultPoint:), alignmentFeedbackTokenForHorizontalMovement(in:previousX:alignedX:defaultX:), or alignmentFeedbackTokenForVerticalMovement(in:previousY:alignedY:defaultY:). Typically, no more than one feedback token per dimension (horizontal/vertical) should be provided.

`performanceTime`  

The time, of type `NSHapticFeedbackPerformanceTime`, when the feedback should be provided to the user.

## Discussion

Call this method to initiate haptic feedback to the user. Pass it one or more alignment feedback tokens of type `NSAlignmentFeedbackToken` and a time to execute of type `NSHapticFeedbackPerformanceTime`. Call this method immediately before moving the object to its new aligned position.

## See Also

### Related Documentation

protocol NSHapticFeedbackPerformer

A set of methods and constants that a haptic feedback performer implements.

enum PerformanceTime

A time at which to provide haptic feedback to the user.

