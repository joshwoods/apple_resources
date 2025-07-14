

- UIKit
- UIContextMenuConfiguration
-  UIContextMenuConfiguration.ElementOrder 

Enumeration

# UIContextMenuConfiguration.ElementOrder

Constants that define the ordering strategy for menu elements in a context menu.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 17.0+visionOS 1.0+

``` source
enum ElementOrder
```

## Topics

### Constants

case automatic

A constant that allows the system to choose an ordering strategy according to the current context.

case priority

A constant that displays menu elements according to their priority.

case fixed

A constant that displays menu elements in a fixed order.

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

### Specifying the order of menu elements

var preferredMenuElementOrder: UIContextMenuConfiguration.ElementOrder

The preferred menu-element ordering strategy for the menu.

