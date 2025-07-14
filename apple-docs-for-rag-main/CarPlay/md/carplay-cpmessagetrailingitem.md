

- CarPlay
-  CPMessageTrailingItem 

Enumeration

# CPMessageTrailingItem

The accessories that a message list item can display in its trailing region.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+

``` source
enum CPMessageTrailingItem
```

## Overview

Use these constants when creating instances of CPMessageListItemTrailingConfiguration. A trailing item can provide additional context for a list item’s contents, or help communicate its behavior.

## Topics

### Trailing Items

case none

Don’t show a trailing item.

case mute

Show a muted speaker icon.

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

### Getting the Trailing Item

var trailingItem: CPMessageTrailingItem

The configuration’s item.

