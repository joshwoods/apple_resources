

- UIKit
- UIWindow
-  didBecomeHiddenNotification 

Type Property

# didBecomeHiddenNotification

A notification that posts when a window becomes hidden.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let didBecomeHiddenNotification: NSNotification.Name
```

## Discussion

The notification object is the hidden window. This notification doesn’t contain a `userInfo` dictionary.

Switching between apps doesn’t generate visibility-related notifications for windows. Window visibility changes reflect changes to the window’s isHidden property and reflect only the window’s visibility within the app.

The system posts this notification on the main actor.

## See Also

### Responding to window-related notifications

class let didBecomeVisibleNotification: NSNotification.Name

A notification that posts when a window becomes visible.

class let didBecomeKeyNotification: NSNotification.Name

A notification that posts whenever a window becomes the key window.

class let didResignKeyNotification: NSNotification.Name

A notification that posts whenever a window resigns its status as main window.

