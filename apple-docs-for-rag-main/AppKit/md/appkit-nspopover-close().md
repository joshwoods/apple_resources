

- AppKit
- NSPopover
-  close() 

Instance Method

# close()

Forces the popover to close without consulting its delegate.

macOS 10.7+

``` source
@MainActor
func close()
```

## Discussion

Any popovers nested within the popovers will also receive a close() message. When a window is closed in response to the close() message being sent, all of its popovers are closed. The popover animates out when closed unless the animates property is set to false.

## See Also

### Closing a Popover

func performClose(Any?)

Attempts to close the popover.

