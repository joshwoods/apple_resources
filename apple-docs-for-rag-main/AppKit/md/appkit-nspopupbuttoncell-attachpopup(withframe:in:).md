

- AppKit
- NSPopUpButtonCell
-  attachPopUp(withFrame:in:) 

Instance Method

# attachPopUp(withFrame:in:)

Sets up the receiver to display a menu.

macOS

``` source
@MainActor
func attachPopUp(
    withFrame cellFrame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`cellFrame`  

The cell’s rectangle, specified in points in the coordinate system of the view in the `controlView` parameter. The menu is attached to this rectangle.

`controlView`  

The view in which to display the pop-up button’s menu.

## Discussion

This call sets up the popup button cell to display a menu, which occurs in performClick(withFrame:in:). This method sets the cell’s control view and then highlights and redraws the cell. It does not show the menu.

This method also posts an willPopUpNotification. (The `NSPopUpButton` object sends a corresponding willPopUpNotification.)

You normally do not call this method explicitly. It is called by the Application Kit automatically when the menu for the pop-up button is to be displayed.

## See Also

### Handling events and action messages

func dismissPopUp()

Dismisses the pop-up button’s menu by ordering its window out.

func performClick(withFrame: NSRect, in: NSView)

Displays the receiver’s menu and track mouse events in it.

