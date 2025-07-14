

- AppKit
- NSButtonCell
-  performClick(\_:) 

Instance Method

# performClick(\_:)

Simulates the user clicking the button with the pointer.

macOS

``` source
@MainActor
func performClick(_ sender: Any?)
```

## Parameters 

`sender`  

The sender of the message.

## Discussion

This method essentially highlights the button, sends the button’s action message to the target object, and then unhighlights the button.

If an exception is raised while the target object is processing the action message, the button is unhighlighted before the exception is propagated out of performClick(_:).

## See Also

### Handling Events and Action Messages

func mouseEntered(with: NSEvent)

Draws the button’s border.

func mouseExited(with: NSEvent)

Erases the button’s border.

