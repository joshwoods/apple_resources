

- SwiftUI
- TableColumnAlignment
-  trailing 

Type Property

# trailing

Trailing column alignment.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static var trailing: TableColumnAlignment { get }
```

## Discussion

With a `layoutDirection` of `leftToRight`, this is equivalent to right; and with a `layoutDirection` of `rightToLeft`, this is equivalent to left.

## See Also

### Getting the alignment

static var automatic: TableColumnAlignment

The default column alignment.

static var leading: TableColumnAlignment

Leading column alignment.

static var center: TableColumnAlignment

Center column alignment.

static var numeric: TableColumnAlignment

Column alignment appropriate for numeric content.

static func numeric(Locale.NumberingSystem) -> TableColumnAlignment

Column alignment appropriate for numeric content.

