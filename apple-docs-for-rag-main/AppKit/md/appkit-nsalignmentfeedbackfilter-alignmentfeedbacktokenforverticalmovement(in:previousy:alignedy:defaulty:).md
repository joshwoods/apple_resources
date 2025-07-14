

- AppKit
- NSAlignmentFeedbackFilter
-  alignmentFeedbackTokenForVerticalMovement(in:previousY:alignedY:defaultY:) 

Instance Method

# alignmentFeedbackTokenForVerticalMovement(in:previousY:alignedY:defaultY:)

Requests a feedback token for the alignment of an object requiring vertical movement only.

macOS 10.11+

``` source
func alignmentFeedbackTokenForVerticalMovement(
    in view: NSView?,
    previousY: CGFloat,
    alignedY: CGFloat,
    defaultY: CGFloat
) -> (any NSAlignmentFeedbackToken)?
```

## Parameters 

`view`  

The view (NSView) in which the object was moved.

`previousY`  

The vertical location (CGFloat) of the object prior to its move.

`alignedY`  

The new vertical location (CGFloat) of the object if alignment occurs.

`defaultY`  

The current vertical location (CGFloat) of the object. This is where the user actually moved the object. This location may be offset from the location of the cursor.

## Return Value

If the system determines that the alignment should not occur, a null value is returned. Otherwise, a feedback token of type `NSAlignmentFeedbackToken` is returned.

## Discussion

This method requests a feedback token for the alignment of an object requiring vertical movement only.

If a feedback token is returned, call performFeedback(_:performanceTime:) to initiate haptic feedback. Then, move the object to its aligned location.

If no feedback token is returned, don’t perform the vertical alignment or request haptic feedback. Even if this vertical alignment fails, be sure to check other alignments. For example, a horizontal alignment may still be allowed. If no alignments will occur, move the object to its default location.

## See Also

### Related Documentation

func performFeedback([any NSAlignmentFeedbackToken], performanceTime: NSHapticFeedbackManager.PerformanceTime)

Performs the haptic feedback described by one or more alignment feedback tokens.

### Preparing Haptic Feedback for Alignment

func alignmentFeedbackTokenForMovement(in: NSView?, previousPoint: NSPoint, alignedPoint: NSPoint, defaultPoint: NSPoint) -> (any NSAlignmentFeedbackToken)?

Requests a feedback token for the alignment of an object requiring horizontal and vertical movement.

func alignmentFeedbackTokenForHorizontalMovement(in: NSView?, previousX: CGFloat, alignedX: CGFloat, defaultX: CGFloat) -> (any NSAlignmentFeedbackToken)?

Requests a feedback token for the alignment of an object requiring horizontal movement only.

