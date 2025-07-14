

- UIKit
- UITextLoupeSession
-  move(to:withCaretRect:trackingCaret:) 

Instance Method

# move(to:withCaretRect:trackingCaret:)

Moves the loupe to the specified point in the session’s associated view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+

``` source
@MainActor
func move(
    to point: CGPoint,
    withCaretRect caretRect: CGRect,
    trackingCaret tracksCaret: Bool
)
```

## Parameters 

`point`  

The new location you want to magnify with the loupe. When creating the loupe with a gesture recognizer, specify the location of the gesture.

`caretRect`  

The current position of the caret handle. Specify CGRectNull if the view doesn’t contain a selection or the caret isn’t visible.

`tracksCaret`  

`true` if you want the loupe to track the movements of the caret. If you specify `true`, provide a valid rectangle in the `caretRect` parameter. Specify `false` to continue tracking the location of touch events.

## Mentioned in 

Adopting system selection UI in custom text views

## Discussion

Call this method repeatedly from a gesture recognizer when the touch location changes.

## See Also

### Updating the loupe during the session

func invalidate()

Hides the loupe and cleans up any session-related state.

