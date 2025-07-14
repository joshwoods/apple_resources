

- UIKit
-  UIFocusItemDeferralMode 

Enumeration

# UIFocusItemDeferralMode

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
enum UIFocusItemDeferralMode
```

## Topics

### Enumeration Cases

case always

Always defer focus for this item, even if deferral is disabled right now. This means a programmatic update to this item would result in focus disappearing until the user interacts with the focus engine again.

case automatic

Use the system default behavior.

case never

Never defer focus for this item. When a programmatic focus update lands on this item, it will always be and appear focused even if focus deferral is currently enabled.

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

### Enumerations

enum ExpandedStatus

enum ComponentSize

