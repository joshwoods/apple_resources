

- UIKit
- UITextLoupeSession
-  invalidate() 

Instance Method

# invalidate()

Hides the loupe and cleans up any session-related state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+

``` source
@MainActor
func invalidate()
```

## Mentioned in 

Adopting system selection UI in custom text views

## Discussion

Call this method when you’re ready to hide the loupe. After calling this method, you can remove your reference to the session.

## See Also

### Updating the loupe during the session

func move(to: CGPoint, withCaretRect: CGRect, trackingCaret: Bool)

Moves the loupe to the specified point in the session’s associated view.

