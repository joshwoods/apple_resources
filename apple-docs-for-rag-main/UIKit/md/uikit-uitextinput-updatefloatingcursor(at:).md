

- UIKit
- UITextInput
-  updateFloatingCursor(at:) 

Instance Method

# updateFloatingCursor(at:)

Tells the object that the floating cursor moved to a new location.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func updateFloatingCursor(at point: CGPoint)
```

## Parameters 

`point`  

The new touch point in the underlying view. This point is in the coordinate space of the view in the textInputView property.

## Discussion

UIKit calls this method when the touch location changes for the two-finger pan gesture used to move the cursor. You can use this method to update the visual state of your text view. For example, you might use this method to display custom visual feedback for cursor movements.This method may be called multiple times while the user’s fingers are moving, so your implementation should be fast. If you do not implement this method, UIKit provides visual feedback only when the selection changes.

## See Also

### Managing the floating cursor

func beginFloatingCursor(at: CGPoint)

Tells the object when the gesture that the system uses to manipulate the cursor begins.

func endFloatingCursor()

Tells the object when the gesture that the system uses to manipulate the cursor ends.

