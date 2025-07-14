

- AppKit
- NSBrowser
-  takesTitleFromPreviousColumn 

Instance Property

# takesTitleFromPreviousColumn

A Boolean that indicates whether a column takes its title from the selected cell in the previous column.

macOS

``` source
@MainActor
var takesTitleFromPreviousColumn: Bool { get set }
```

## Discussion

When the value of this property is true, the title of a column is set to the string value of the selected `NSCell` in the previous column.

## See Also

### Configuring Browsers

var reusesColumns: Bool

A Boolean that indicates whether the browser reuses matrix objects after their columns are unloaded.

var maxVisibleColumns: Int

The maximum number of visible columns.

var autohidesScroller: Bool

A Boolean that indicates whether the browser automatically hides its scroller.

var backgroundColor: NSColor

The browser’s background color.

var minColumnWidth: CGFloat

The minimum column width, in pixels.

var separatesColumns: Bool

A Boolean that indicates whether columns are separated by bezeled borders.

func tile()

Adjusts the various subviews of the browser—scrollers, columns, titles, and so on—without redrawing.

var delegate: (any NSBrowserDelegate)?

The browser’s delegate.

