

- WatchKit
- WKInterfaceTable
-  curvesAtBottom 

Instance Property

# curvesAtBottom

A Boolean value that determines whether the rows shrink to match the curved corners at the bottom of the screen.

watchOS 5.1+

``` source
var curvesAtBottom: Bool { get set }
```

## Discussion

Defaults to false. If true, table rows near the bottom of the screen shrink so that the curved corners don’t clip them. This property has no effect on Apple Watch Series 3 or earlier.

## See Also

### Scrolling

func scrollToRow(at: Int)

Scrolls the row at the specified index into view.

var curvesAtTop: Bool

A Boolean value that determines whether the rows shrink to match the curved corners at the top of the screen.

