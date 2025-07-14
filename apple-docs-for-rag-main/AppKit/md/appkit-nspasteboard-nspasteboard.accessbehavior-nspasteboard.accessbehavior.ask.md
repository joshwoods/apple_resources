

- AppKit
- NSPasteboard
- NSPasteboard.AccessBehavior
-  NSPasteboard.AccessBehavior.ask 

Case

# NSPasteboard.AccessBehavior.ask

The system will notify the user and ask for permission before granting pasteboard access. However, access that is both user originated and paste related will always be allowed, and will not result in a notification. The app is listed in the corresponding System Settings pane.

macOS 15.4+

``` source
case ask
```

