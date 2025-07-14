

- AppKit
- NSPopover
-  NSPopover.CloseReason 

Structure

# NSPopover.CloseReason

Values that specify the reason for the willCloseNotification notification.

macOS

``` source
struct CloseReason
```

## Topics

### Constants

static let detachToWindow: NSPopover.CloseReason

Specifies that the popover has been closed because it is being detached to a window.

static let standard: NSPopover.CloseReason

Specifies that the popover has been closed in a standard way.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Behavior

The appearance and disappearance behavior of a popover.

class let closeReasonUserInfoKey: String

The `userInfo` key containing the reason for the willCloseNotification.

enum Appearance

The set of predefined appearances for a popover.

Deprecated

