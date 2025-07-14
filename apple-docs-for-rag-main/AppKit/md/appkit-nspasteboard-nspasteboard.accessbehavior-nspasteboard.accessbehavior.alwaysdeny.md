

- AppKit
- NSPasteboard
- NSPasteboard.AccessBehavior
-  NSPasteboard.AccessBehavior.alwaysDeny 

Case

# NSPasteboard.AccessBehavior.alwaysDeny

The system will automatically deny all pasteboard access, without notifying the user. However, access that is both user originated and paste related will always be allowed, and will not result in a notification. The app is listed in the corresponding System Settings pane.

macOS 15.4+

``` source
case alwaysDeny
```

