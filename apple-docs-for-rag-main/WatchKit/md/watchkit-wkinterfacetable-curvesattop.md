

- WatchKit
- WKInterfaceTable
-  curvesAtTop 

Instance Property

# curvesAtTop

A Boolean value that determines whether the rows shrink to match the curved corners at the top of the screen.

watchOS 5.1+

``` source
var curvesAtTop: Bool { get set }
```

## Discussion

Defaults to false. If true, table rows near the top of the screen shrink so that the curved corners don’t clip them. Typically, this property has no effect when the status bar is visible. It also has no effect on Apple Watch Series 3 or earlier.

## See Also

### Scrolling

func scrollToRow(at: Int)

Scrolls the row at the specified index into view.

var curvesAtBottom: Bool

A Boolean value that determines whether the rows shrink to match the curved corners at the bottom of the screen.

