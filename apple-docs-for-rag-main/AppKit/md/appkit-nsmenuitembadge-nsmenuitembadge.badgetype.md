

- AppKit
- NSMenuItemBadge
-  NSMenuItemBadge.BadgeType 

Enumeration

# NSMenuItemBadge.BadgeType

Constants that define types of badges for display.

macOS 14.0+

``` source
enum BadgeType
```

## Overview

The predefined strings that display are localizable and automatically handle any pluralization of itemCount.

## Topics

### Getting badge types

case alerts

A badge representing the number of alerts.

case newItems

A badge representing the number of new items.

case none

A badge with no string portion.

case updates

A badge representing the number of available updates.

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

### Creating badges of a specific type

class func alerts(count: Int) -> Self

Creates an alert-style badge with an integer count and a predefined label that represents the number of alerts.

class func newItems(count: Int) -> Self

Creates a new item-style badge with an integer count and a predefined label that represents the number of new items.

class func updates(count: Int) -> Self

Creates an update-style badge with an integer count and a predefined label that represents the number of available updates.

