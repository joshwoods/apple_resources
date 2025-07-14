

- AppKit
-  NSTextMovement 

Enumeration

# NSTextMovement

macOS

``` source
enum NSTextMovement
```

## Topics

### Movement Options

case `return`

case tab

case backtab

case left

case right

case up

case down

case cancel

case other

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

### Notifications

class let didBeginEditingNotification: NSNotification.Name

Posted when an `NSText` object begins any operation that changes characters or formatting attributes.

class let didChangeNotification: NSNotification.Name

Posted after an `NSText` object performs any operation that changes characters or formatting attributes.

class let didEndEditingNotification: NSNotification.Name

Posted when focus leaves an `NSText` object, whether or not any operation has changed characters or formatting attributes.

class let movementUserInfoKey: String

The `userInfo` dictionary key for the didEndEditingNotification notification.

