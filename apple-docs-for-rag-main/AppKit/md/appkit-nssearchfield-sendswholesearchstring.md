

- AppKit
- NSSearchField
-  sendsWholeSearchString 

Instance Property

# sendsWholeSearchString

A Boolean value indicating whether the cell calls its search action method when the user clicks the search button or presses Return, or after each keystroke.

macOS 10.10+

``` source
@MainActor
var sendsWholeSearchString: Bool { get set }
```

## Discussion

When the value of this property is yes, the field calls its action method when the user clicks the search button or presses Return. When the value is NO, the field calls the action method after each keystroke. The default value of this property is no.

## See Also

### Managing Search Modes

var sendsSearchStringImmediately: Bool

A Boolean value indicating whether the cell calls its action method immediately when an appropriate action occurs.

