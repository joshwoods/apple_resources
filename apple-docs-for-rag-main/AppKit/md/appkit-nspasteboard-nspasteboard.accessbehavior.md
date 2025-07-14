

- AppKit
- NSPasteboard
-  NSPasteboard.AccessBehavior 

Enumeration

# NSPasteboard.AccessBehavior

A value indicating pasteboard access behavior.

macOS 15.4+

``` source
enum AccessBehavior
```

## Topics

### Enumeration Cases

case alwaysAllow

The system will automatically allow all pasteboard access, without notifying the user. The app is listed in the corresponding System Settings pane.

case alwaysDeny

The system will automatically deny all pasteboard access, without notifying the user. However, access that is both user originated and paste related will always be allowed, and will not result in a notification. The app is listed in the corresponding System Settings pane.

case ask

The system will notify the user and ask for permission before granting pasteboard access. However, access that is both user originated and paste related will always be allowed, and will not result in a notification. The app is listed in the corresponding System Settings pane.

case `default`

The default behavior for the General pasteboard is to ask upon programmatic access. All other pasteboards default to always allow access. If an app has never triggered a pasteboard access alert, its General pasteboard will report `.default` behavior. Such an app is not shown in the corresponding System Settings pane. Once programmatic pasteboard access triggers the first pasteboard access alert, the state automatically changes to `.ask`. At this point the app starts being shown in System Settings, where the user can toggle the behavior between `.ask`, `.alwaysAllow`, and `.alwaysDeny`.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

