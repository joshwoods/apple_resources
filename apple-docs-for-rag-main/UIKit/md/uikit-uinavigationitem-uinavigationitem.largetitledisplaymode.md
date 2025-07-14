

- UIKit
- UINavigationItem
-  UINavigationItem.LargeTitleDisplayMode 

Enumeration

# UINavigationItem.LargeTitleDisplayMode

Constants that indicate how to size the title of this item.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum LargeTitleDisplayMode
```

## Topics

### Constants

case automatic

Inherit the display mode from the previous navigation item.

case always

Always display a large title.

case never

Never display a large title.

### Enumeration Cases

case inline

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

### Configuring the title

var title: String?

The navigation item’s title that displays in the navigation bar.

var largeTitleDisplayMode: UINavigationItem.LargeTitleDisplayMode

The mode for displaying the title of the navigation bar.

