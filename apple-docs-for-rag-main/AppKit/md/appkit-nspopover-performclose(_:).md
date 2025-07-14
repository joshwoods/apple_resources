

- AppKit
- NSPopover
-  performClose(\_:) 

Instance Method

# performClose(\_:)

Attempts to close the popover.

macOS 10.7+

``` source
@IBAction @MainActor
func performClose(_ sender: Any?)
```

## Parameters 

`sender`  

The sender of the action message.

## Discussion

The popover will not be closed if it has a delegate and the delegate implements the returns popoverShouldClose(_:) method returning false, or if a subclass of the NSPopover class implements `popoverShouldClose:` and returns false).

The operation will fail if the popover is displaying a nested popover or if it has a child window. A window will attempt to close its popovers when it receives a performClose(_:) message.

The popover animates out when closed unless the animates property is set to false.

## See Also

### Closing a Popover

func close()

Forces the popover to close without consulting its delegate.

