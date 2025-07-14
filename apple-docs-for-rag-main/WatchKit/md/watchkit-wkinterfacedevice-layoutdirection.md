

- WatchKit
- WKInterfaceDevice
-  layoutDirection 

Instance Property

# layoutDirection

The layout direction of the user interface.

watchOS 2.1+

``` source
var layoutDirection: WKInterfaceLayoutDirection { get }
```

## Discussion

For a list of possible values, see WKInterfaceLayoutDirection.

## See Also

### Accessing the Layout Direction

class func interfaceLayoutDirection(for: WKInterfaceSemanticContentAttribute) -> WKInterfaceLayoutDirection

Returns the user interface direction for the given semantic content attribute.

enum WKInterfaceSemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

enum WKInterfaceLayoutDirection

Specifies the directional flow of the user interface.

