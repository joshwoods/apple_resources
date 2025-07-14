

- AppKit
- NSPopover
-  willCloseNotification 

Type Property

# willCloseNotification

Sent before the popover is closed.

macOS 10.7+

``` source
class let willCloseNotification: NSNotification.Name
```

## Discussion

The `userInfo` key closeReasonUserInfoKey specifies the reason for closing. It can currently be either standard or detachToWindow, although more reasons for closing may be added in the future.

## See Also

### Notifications

class let willShowNotification: NSNotification.Name

Sent before the popover is shown.

class let didShowNotification: NSNotification.Name

Sent after the popover has finished animating onscreen.

class let didCloseNotification: NSNotification.Name

Sent after the popover has finished animating offscreen.

