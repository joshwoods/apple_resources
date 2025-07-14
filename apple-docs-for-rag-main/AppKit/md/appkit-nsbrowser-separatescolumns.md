

- AppKit
- NSBrowser
-  separatesColumns 

Instance Property

# separatesColumns

A Boolean that indicates whether columns are separated by bezeled borders.

macOS

``` source
@MainActor
var separatesColumns: Bool { get set }
```

## Discussion

When the value of this property is true, the browser’s columns are separated by bezeled borders.

This value is ignored if isTitled does not return false.

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

var takesTitleFromPreviousColumn: Bool

A Boolean that indicates whether a column takes its title from the selected cell in the previous column.

func tile()

Adjusts the various subviews of the browser—scrollers, columns, titles, and so on—without redrawing.

var delegate: (any NSBrowserDelegate)?

The browser’s delegate.

