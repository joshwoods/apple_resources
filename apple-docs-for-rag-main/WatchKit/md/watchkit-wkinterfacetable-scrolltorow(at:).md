

- WatchKit
- WKInterfaceTable
-  scrollToRow(at:) 

Instance Method

# scrollToRow(at:)

Scrolls the row at the specified index into view.

watchOS 2.0+

``` source
func scrollToRow(at index: Int)
```

## Parameters 

`index`  

The index of the row to be displayed. Specifying an index less than `0` scrolls to the top of the list. Specifying an index greater than the total number of row controllers scrolls to the bottom of the list.

## See Also

### Scrolling

var curvesAtBottom: Bool

A Boolean value that determines whether the rows shrink to match the curved corners at the bottom of the screen.

var curvesAtTop: Bool

A Boolean value that determines whether the rows shrink to match the curved corners at the top of the screen.

