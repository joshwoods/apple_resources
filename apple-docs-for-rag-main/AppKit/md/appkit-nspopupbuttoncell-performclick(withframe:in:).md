

- AppKit
- NSPopUpButtonCell
-  performClick(withFrame:in:) 

Instance Method

# performClick(withFrame:in:)

Displays the receiver’s menu and track mouse events in it.

macOS

``` source
@MainActor
func performClick(
    withFrame frame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`frame`  

The cell’s rectangle, specified in points in the coordinate system of the view in the `controlView` parameter.

`controlView`  

The view in which to display the pop-up button’s menu.

## Discussion

You normally do not call this method explicitly. It is called by the Application Kit automatically to handle events in the pop-up button.

## See Also

### Handling events and action messages

func attachPopUp(withFrame: NSRect, in: NSView)

Sets up the receiver to display a menu.

func dismissPopUp()

Dismisses the pop-up button’s menu by ordering its window out.

