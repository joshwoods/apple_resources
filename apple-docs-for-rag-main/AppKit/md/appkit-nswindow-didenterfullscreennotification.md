

- AppKit
- NSWindow
-  didEnterFullScreenNotification 

Type Property

# didEnterFullScreenNotification

A notification that the window entered full-screen mode.

macOS 10.7+

``` source
class let didEnterFullScreenNotification: NSNotification.Name
```

## Discussion

The notification object is the `NSWindow` object that entered full-screen mode. This notification doesn’t contain a `userInfo` dictionary.

## See Also

### Notifications

class let didBecomeKeyNotification: NSNotification.Name

A notification that the window object became the key window.

class let didBecomeMainNotification: NSNotification.Name

A notification that the window object became the main window.

class let didChangeScreenNotification: NSNotification.Name

A notification that a portion of the window object’s frame moved onto or off of a screen.

class let didChangeScreenProfileNotification: NSNotification.Name

A notification that the screen containing the window changed.

class let didDeminiaturizeNotification: NSNotification.Name

A notification that the window is no longer minimized.

class let didEndSheetNotification: NSNotification.Name

A notification that the window object closed an attached sheet.

class let didEndLiveResizeNotification: NSNotification.Name

A notification that the user resized the window object.

class let didExposeNotification: NSNotification.Name

A notification that a window exposed a portion of its nonretained content.

class let didMiniaturizeNotification: NSNotification.Name

A notification that the window object minimized.

class let didMoveNotification: NSNotification.Name

A notification that the window object moved.

class let didResignKeyNotification: NSNotification.Name

A notification that the window object resigned its status as key window.

class let didResignMainNotification: NSNotification.Name

A notification that the window object resigned its status as main window.

class let didResizeNotification: NSNotification.Name

A notification that the window object size changed.

class let didUpdateNotification: NSNotification.Name

A notification that the window object received an update message.

class let willBeginSheetNotification: NSNotification.Name

A notification that the window object is about to open a sheet.

