

- AppKit
- NSPopover
-  didCloseNotification 

Type Property

# didCloseNotification

Sent after the popover has finished animating offscreen.

macOS 10.7+

``` source
class let didCloseNotification: NSNotification.Name
```

## Discussion

The value of the `userInfo` key closeReasonUserInfoKey specifies the reason for closing. It can currently be either standard or detachToWindow, although more reasons for closing may be added in the future.

## See Also

### Notifications

class let willShowNotification: NSNotification.Name

Sent before the popover is shown.

class let didShowNotification: NSNotification.Name

Sent after the popover has finished animating onscreen.

class let willCloseNotification: NSNotification.Name

Sent before the popover is closed.

