

- AppKit
- NSBrowser
-  clickedColumn 

Instance Property

# clickedColumn

The column number of the cell that the user clicked to display a context menu.

macOS 10.6+

``` source
@MainActor
var clickedColumn: Int { get }
```

## Discussion

The value of this property is `-1` if no context menu is active.

## See Also

### Handling Mouse-Click Events

func doClick(Any?)

Responds to (single) mouse clicks in a column of the browser.

func doDoubleClick(Any?)

Responds to double clicks in a column of the browser.

var clickedRow: Int

The row number of the cell that the user clicked to display a context menu.

