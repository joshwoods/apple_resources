

- AppKit
- NSSearchField
-  sendsSearchStringImmediately 

Instance Property

# sendsSearchStringImmediately

A Boolean value indicating whether the cell calls its action method immediately when an appropriate action occurs.

macOS 10.10+

``` source
@MainActor
var sendsSearchStringImmediately: Bool { get set }
```

## Discussion

When the value of this property is YES, the field calls its action method immediately upon notification of any changes to the search field. When the value is NO, the field pauses briefly after receiving a notification and then calls its action method. Pausing gives the user an opportunity to type more text into the search field and minimize the number of searches that are performed.

## See Also

### Managing Search Modes

var sendsWholeSearchString: Bool

A Boolean value indicating whether the cell calls its search action method when the user clicks the search button or presses Return, or after each keystroke.

