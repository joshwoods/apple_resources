

- AppKit
- NSAlignmentFeedbackFilter
-  alignmentFeedbackTokenForMovement(in:previousPoint:alignedPoint:defaultPoint:) 

Instance Method

# alignmentFeedbackTokenForMovement(in:previousPoint:alignedPoint:defaultPoint:)

Requests a feedback token for the alignment of an object requiring horizontal and vertical movement.

macOS 10.11+

``` source
func alignmentFeedbackTokenForMovement(
    in view: NSView?,
    previousPoint: NSPoint,
    alignedPoint: NSPoint,
    defaultPoint: NSPoint
) -> (any NSAlignmentFeedbackToken)?
```

## Parameters 

`view`  

The view (NSView) in which the object was moved.

`previousPoint`  

The location (NSPoint) of the object prior to its move.

`alignedPoint`  

The new location (NSPoint) of the object if alignment occurs.

`defaultPoint`  

The current location (NSPoint) of the object. This is where the user actually moved the object. This location may be offset from the location of the cursor.

## Return Value

A null value if the system determines that the alignment should not occur. Otherwise, a feedback token of type `NSAlignmentFeedbackToken` is returned.

## Discussion

This method requests a feedback token for the alignment of an object requiring horizontal and vertical movement.

If a feedback token is returned, call performFeedback(_:performanceTime:) to initiate haptic feedback. Then, move the object to its aligned location.

If no feedback token is returned, don’t perform the alignment or request haptic feedback. Even if this joint horizontal and vertical alignment fails, be sure to check other alignments. For example, an individual horizontal or vertical alignment may still be allowed. If no alignments will occur, move the object to its default location.

## See Also

### Related Documentation

func performFeedback([any NSAlignmentFeedbackToken], performanceTime: NSHapticFeedbackManager.PerformanceTime)

Performs the haptic feedback described by one or more alignment feedback tokens.

### Preparing Haptic Feedback for Alignment

func alignmentFeedbackTokenForHorizontalMovement(in: NSView?, previousX: CGFloat, alignedX: CGFloat, defaultX: CGFloat) -> (any NSAlignmentFeedbackToken)?

Requests a feedback token for the alignment of an object requiring horizontal movement only.

func alignmentFeedbackTokenForVerticalMovement(in: NSView?, previousY: CGFloat, alignedY: CGFloat, defaultY: CGFloat) -> (any NSAlignmentFeedbackToken)?

Requests a feedback token for the alignment of an object requiring vertical movement only.

