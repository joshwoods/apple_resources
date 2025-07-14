

- AppKit
- NSBrowser
-  backgroundColor 

Instance Property

# backgroundColor

The browser’s background color.

macOS 10.5+

``` source
@MainActor
var backgroundColor: NSColor { get set }
```

## Discussion

The default value of this property is `[NSColor whiteColor]`. `[NSColor clearColor]` specifies a transparent background.

## See Also

### Configuring Browsers

var reusesColumns: Bool

A Boolean that indicates whether the browser reuses matrix objects after their columns are unloaded.

var maxVisibleColumns: Int

The maximum number of visible columns.

var autohidesScroller: Bool

A Boolean that indicates whether the browser automatically hides its scroller.

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

