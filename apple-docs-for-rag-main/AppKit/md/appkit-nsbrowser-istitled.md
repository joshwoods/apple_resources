

- AppKit
- NSBrowser
-  isTitled 

Instance Property

# isTitled

A Boolean that indicates whether columns display titles.

macOS

``` source
@MainActor
var isTitled: Bool { get set }
```

## Discussion

When the value of this property is true, the columns in a browser display titles.

## See Also

### Accessing Column Titles

func title(ofColumn: Int) -> String?

Returns the title displayed for the given column.

func setTitle(String, ofColumn: Int)

Sets the title of the given column.

func drawTitle(ofColumn: Int, in: NSRect)

Draws the title for the specified column within the given rectangle.

var titleHeight: CGFloat

The height of the column titles for the browser.

func titleFrame(ofColumn: Int) -> NSRect

Returns the bounds of the title frame for the specified column.

