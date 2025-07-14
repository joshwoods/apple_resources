

- AppKit
- NSBrowser
-  setTitle(\_:ofColumn:) 

Instance Method

# setTitle(\_:ofColumn:)

Sets the title of the given column.

macOS

``` source
@MainActor
func setTitle(
    _ string: String,
    ofColumn column: Int
)
```

## Parameters 

`string`  

The title of the column.

`column`  

The index of the column whose title should be set.

## See Also

### Accessing Column Titles

func title(ofColumn: Int) -> String?

Returns the title displayed for the given column.

var isTitled: Bool

A Boolean that indicates whether columns display titles.

func drawTitle(ofColumn: Int, in: NSRect)

Draws the title for the specified column within the given rectangle.

var titleHeight: CGFloat

The height of the column titles for the browser.

func titleFrame(ofColumn: Int) -> NSRect

Returns the bounds of the title frame for the specified column.

