

- AppKit
- NSBrowser
-  titleHeight 

Instance Property

# titleHeight

The height of the column titles for the browser.

macOS

``` source
@MainActor
var titleHeight: CGFloat { get }
```

## See Also

### Accessing Column Titles

func title(ofColumn: Int) -> String?

Returns the title displayed for the given column.

func setTitle(String, ofColumn: Int)

Sets the title of the given column.

var isTitled: Bool

A Boolean that indicates whether columns display titles.

func drawTitle(ofColumn: Int, in: NSRect)

Draws the title for the specified column within the given rectangle.

func titleFrame(ofColumn: Int) -> NSRect

Returns the bounds of the title frame for the specified column.

