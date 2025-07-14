

- UIKit
- UITabBar
-  UITabBar.ItemPositioning 

Enumeration

# UITabBar.ItemPositioning

Constants that specify tab bar item positioning.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum ItemPositioning
```

## Topics

### Constants

case automatic

Specifies automatic tab bar item positioning according to the user interface idiom, as follows:

case fill

Distribute items across the entire width of the tab bar.

case centered

Center items in the available space.

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

### Customizing item spacing

var itemPositioning: UITabBar.ItemPositioning

The positioning scheme for the tab bar items in the tab bar.

var itemSpacing: CGFloat

The amount of space (in points) to use between tab bar items.

var itemWidth: CGFloat

The width (in points) of tab bar items.

