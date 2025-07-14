

- AppKit
- NSBrowser
-  autohidesScroller 

Instance Property

# autohidesScroller

A Boolean that indicates whether the browser automatically hides its scroller.

macOS 10.6+

``` source
@MainActor
var autohidesScroller: Bool { get set }
```

## Discussion

When the value of this property is true, the scroller is automatically hidden.

## See Also

### Configuring Browsers

var reusesColumns: Bool

A Boolean that indicates whether the browser reuses matrix objects after their columns are unloaded.

var maxVisibleColumns: Int

The maximum number of visible columns.

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

