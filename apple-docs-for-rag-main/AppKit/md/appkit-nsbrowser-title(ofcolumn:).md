

- AppKit
- NSBrowser
-  title(ofColumn:) 

Instance Method

# title(ofColumn:)

Returns the title displayed for the given column.

macOS

``` source
@MainActor
func title(ofColumn column: Int) -> String?
```

## Parameters 

`column`  

The index of the column for which to get the title.

## Return Value

The title of the specified column.

## See Also

### Accessing Column Titles

func setTitle(String, ofColumn: Int)

Sets the title of the given column.

var isTitled: Bool

A Boolean that indicates whether columns display titles.

func drawTitle(ofColumn: Int, in: NSRect)

Draws the title for the specified column within the given rectangle.

var titleHeight: CGFloat

The height of the column titles for the browser.

func titleFrame(ofColumn: Int) -> NSRect

Returns the bounds of the title frame for the specified column.

