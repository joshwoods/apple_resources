

- AppKit
- NSPopover
-  NSPopover.Behavior 

Enumeration

# NSPopover.Behavior

The appearance and disappearance behavior of a popover.

macOS

``` source
enum Behavior
```

## Topics

### Constants

case applicationDefined

Your application assumes responsibility for closing the popover.

case transient

The system will close the popover when the user interacts with a user interface element outside the popover.

case semitransient

The system will close the popover when the user interacts with user interface elements in the window containing the popover’s positioning view.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

class let closeReasonUserInfoKey: String

The `userInfo` key containing the reason for the willCloseNotification.

struct CloseReason

Values that specify the reason for the willCloseNotification notification.

enum Appearance

The set of predefined appearances for a popover.

Deprecated

