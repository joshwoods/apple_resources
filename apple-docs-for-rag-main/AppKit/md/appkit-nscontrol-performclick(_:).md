

- AppKit
- NSControl
-  performClick(\_:) 

Instance Method

# performClick(\_:)

Simulates a single mouse click on the receiver.

macOS

``` source
@MainActor
func performClick(_ sender: Any?)
```

## Parameters 

`sender`  

The object requesting the action. This parameter is ignored.

## Discussion

This method calls the performClick(_:) method of the receiver’s cell with the sender being the control itself. This method raises an exception if the action message cannot be successfully sent.

## See Also

### Activating from the Keyboard

var refusesFirstResponder: Bool

A Boolean value indicating whether the receiver refuses the first responder role.

