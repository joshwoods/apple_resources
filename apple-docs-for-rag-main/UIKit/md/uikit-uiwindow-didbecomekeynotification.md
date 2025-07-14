

- UIKit
- UIWindow
-  didBecomeKeyNotification 

Type Property

# didBecomeKeyNotification

A notification that posts whenever a window becomes the key window.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let didBecomeKeyNotification: NSNotification.Name
```

## Discussion

The notification object is the window that became key. This notification doesn’t contain a `userInfo` dictionary.

The system posts this notification on the main actor. In iOS 15 and later, the system posts this notification when the window becomes the key window of its scene. In iOS 14 and earlier, the system posts this notification when the window becomes the key window of the app.

## See Also

### Responding to window-related notifications

class let didBecomeVisibleNotification: NSNotification.Name

A notification that posts when a window becomes visible.

class let didBecomeHiddenNotification: NSNotification.Name

A notification that posts when a window becomes hidden.

class let didResignKeyNotification: NSNotification.Name

A notification that posts whenever a window resigns its status as main window.

