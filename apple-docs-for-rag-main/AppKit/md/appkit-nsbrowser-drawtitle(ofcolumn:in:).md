

- AppKit
- NSBrowser
-  drawTitle(ofColumn:in:) 

Instance Method

# drawTitle(ofColumn:in:)

Draws the title for the specified column within the given rectangle.

macOS

``` source
@MainActor
func drawTitle(
    ofColumn column: Int,
    in rect: NSRect
)
```

## Parameters 

`column`  

The index of the column for which to draw the title.

`rect`  

The rectangle within which to draw the title.

## See Also

### Accessing Column Titles

func title(ofColumn: Int) -> String?

Returns the title displayed for the given column.

func setTitle(String, ofColumn: Int)

Sets the title of the given column.

var isTitled: Bool

A Boolean that indicates whether columns display titles.

var titleHeight: CGFloat

The height of the column titles for the browser.

func titleFrame(ofColumn: Int) -> NSRect

Returns the bounds of the title frame for the specified column.

