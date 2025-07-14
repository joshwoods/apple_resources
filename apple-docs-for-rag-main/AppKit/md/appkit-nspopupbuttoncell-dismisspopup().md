

- AppKit
- NSPopUpButtonCell
-  dismissPopUp() 

Instance Method

# dismissPopUp()

Dismisses the pop-up button’s menu by ordering its window out.

macOS

``` source
@MainActor
func dismissPopUp()
```

## Discussion

If the pop-up button was not displaying its menu, this method does nothing.

You normally do not call this method explicitly. It is called by the Application Kit automatically to dismiss the menu for the pop-up button.

## See Also

### Related Documentation

func orderOut(Any?)

Removes the window from the screen list, which hides the window.

### Handling events and action messages

func attachPopUp(withFrame: NSRect, in: NSView)

Sets up the receiver to display a menu.

func performClick(withFrame: NSRect, in: NSView)

Displays the receiver’s menu and track mouse events in it.

