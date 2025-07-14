

- UIKit
- UITextInput
-  endFloatingCursor() 

Instance Method

# endFloatingCursor()

Tells the object when the gesture that the system uses to manipulate the cursor ends.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func endFloatingCursor()
```

## Discussion

UIKit calls this method at the end of the two-finger pan gesture used to pick up the cursor. You can use this method to clean up the visual state of your text view.

If you do not implement this method, UIKit provides visual feedback only when the selection changes.

## See Also

### Managing the floating cursor

func beginFloatingCursor(at: CGPoint)

Tells the object when the gesture that the system uses to manipulate the cursor begins.

func updateFloatingCursor(at: CGPoint)

Tells the object that the floating cursor moved to a new location.

