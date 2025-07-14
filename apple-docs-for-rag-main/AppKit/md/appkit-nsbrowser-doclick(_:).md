

- AppKit
- NSBrowser
-  doClick(\_:) 

Instance Method

# doClick(\_:)

Responds to (single) mouse clicks in a column of the browser.

macOS

``` source
@MainActor
func doClick(_ sender: Any?)
```

## See Also

### Related Documentation

func sendAction() -> Bool

Sends the action message to the target.

### Handling Mouse-Click Events

func doDoubleClick(Any?)

Responds to double clicks in a column of the browser.

var clickedColumn: Int

The column number of the cell that the user clicked to display a context menu.

var clickedRow: Int

The row number of the cell that the user clicked to display a context menu.

