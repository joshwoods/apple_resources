

- UIKit
- UITextInput
-  beginFloatingCursor(at:) 

Instance Method

# beginFloatingCursor(at:)

Tells the object when the gesture that the system uses to manipulate the cursor begins.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func beginFloatingCursor(at point: CGPoint)
```

## Parameters 

`point`  

The point at which the gesture occurred in your view. This point is in the coordinate space of the view in the textInputView property.

## Discussion

UIKit calls this method when the user begins to perform a two-finger pan gesture to pick up the cursor. You can use this method to update the visual state of your text view. For example, you might use this method to display custom visual feedback for cursor movements.

If you do not implement this method, UIKit provides visual feedback only when the selection changes.

## See Also

### Managing the floating cursor

func updateFloatingCursor(at: CGPoint)

Tells the object that the floating cursor moved to a new location.

func endFloatingCursor()

Tells the object when the gesture that the system uses to manipulate the cursor ends.

