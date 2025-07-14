

- CarPlay
-  CPMessageLeadingItem 

Enumeration

# CPMessageLeadingItem

The accessories that a message list item can display in its leading region.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+

``` source
enum CPMessageLeadingItem
```

## Overview

Use these constants when creating instances of CPMessageListItemLeadingConfiguration. A leading item can provide additional context for a list item’s contents, or help communicate its behavior.

## Topics

### Leading Items

case none

Don’t show a leading item.

case pin

Show a pin icon.

case star

Show a star icon.

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

### Getting the Leading Item

var leadingItem: CPMessageLeadingItem

The configuration’s item.

