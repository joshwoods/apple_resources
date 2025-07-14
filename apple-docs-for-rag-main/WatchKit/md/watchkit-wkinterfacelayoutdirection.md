

- WatchKit
-  WKInterfaceLayoutDirection 

Enumeration

# WKInterfaceLayoutDirection

Specifies the directional flow of the user interface.

watchOS 2.1+

``` source
enum WKInterfaceLayoutDirection
```

## Topics

### Constants

case leftToRight

The layout direction is left-to-right.

case rightToLeft

The layout direction right-to-left. This value is appropriate when your app is running with localizations such as Arabic or Hebrew that should have the user interface layout origin on the right edge of the coordinate system.

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

### Accessing the Layout Direction

var layoutDirection: WKInterfaceLayoutDirection

The layout direction of the user interface.

class func interfaceLayoutDirection(for: WKInterfaceSemanticContentAttribute) -> WKInterfaceLayoutDirection

Returns the user interface direction for the given semantic content attribute.

enum WKInterfaceSemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

