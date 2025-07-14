

- WatchKit
- WKInterfaceDevice
-  interfaceLayoutDirection(for:) 

Type Method

# interfaceLayoutDirection(for:)

Returns the user interface direction for the given semantic content attribute.

watchOS 2.1+

``` source
class func interfaceLayoutDirection(for semanticContentAttribute: WKInterfaceSemanticContentAttribute) -> WKInterfaceLayoutDirection
```

## Parameters 

`semanticContentAttribute`  

The semantic content attribute. For a list of possible values, see WKInterfaceSemanticContentAttribute.

## Return Value

The user interface layout direction (left-to-right or right-to-left). For a list of possible values, see WKInterfaceLayoutDirection.

## See Also

### Accessing the Layout Direction

var layoutDirection: WKInterfaceLayoutDirection

The layout direction of the user interface.

enum WKInterfaceSemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

enum WKInterfaceLayoutDirection

Specifies the directional flow of the user interface.

