

- AppKit
- NSWindowDelegate
-  windowDidChangeBackingProperties(\_:) 

Instance Method

# windowDidChangeBackingProperties(\_:)

Tells the delegate that the window backing properties changed.

macOS 10.7+

``` source
@MainActor
optional func windowDidChangeBackingProperties(_ notification: Notification)
```

## Parameters 

`notification`  

A notification named `NSWindowDidChangeBackingPropertiesNotification`.

## Discussion

You can retrieve the `NSWindow` object in question by sending object to `notification`.

The notification `NSWindowDidChangeBackingPropertiesNotification` is posted in macOS 10.7.3 or later when a window’s backing scale factor or its color space changes. You should watch for this notification instead of `NSWindowDidChangeScreenProfileNotification` if your app runs on a system version on which the backing properties notification is available.

Many apps won’t have the need to watch for this notification, but those that perform sophisticated color handling or manually manage their own cache of window-resolution or color-space-appropriate bitmapped images will find this notification useful as a prompt to invalidate caches or schedule other reassessment for the new resolution or color space. The notification’s `userInfo` dictionary specifies the window’s previous backing scale factor (retrieved with the key`NSBackingPropertyOldScaleFactorKey`) and color space (retrieved with the key `NSBackingPropertyOldColorSpaceKey`). You can compare these with the window’s new previous backing scale factor and color space at the time of the notification to determine which properties changed.

## See Also

### Moving Windows

func windowWillMove(Notification)

Tells the delegate that the window is about to move.

func windowDidMove(Notification)

Tells the delegate that the window has moved.

func windowDidChangeScreen(Notification)

Tells the delegate that the window has changed screens.

func windowDidChangeScreenProfile(Notification)

Tells the delegate that the window has changed screen display profiles.

