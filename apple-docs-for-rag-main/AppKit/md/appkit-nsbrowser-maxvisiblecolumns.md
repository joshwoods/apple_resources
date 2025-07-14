

- AppKit
- NSBrowser
-  maxVisibleColumns 

Instance Property

# maxVisibleColumns

The maximum number of visible columns.

macOS

``` source
@MainActor
var maxVisibleColumns: Int { get set }
```

## See Also

### Configuring Browsers

var reusesColumns: Bool

A Boolean that indicates whether the browser reuses matrix objects after their columns are unloaded.

var autohidesScroller: Bool

A Boolean that indicates whether the browser automatically hides its scroller.

var backgroundColor: NSColor

The browser’s background color.

var minColumnWidth: CGFloat

The minimum column width, in pixels.

var separatesColumns: Bool

A Boolean that indicates whether columns are separated by bezeled borders.

var takesTitleFromPreviousColumn: Bool

A Boolean that indicates whether a column takes its title from the selected cell in the previous column.

func tile()

Adjusts the various subviews of the browser—scrollers, columns, titles, and so on—without redrawing.

var delegate: (any NSBrowserDelegate)?

The browser’s delegate.

