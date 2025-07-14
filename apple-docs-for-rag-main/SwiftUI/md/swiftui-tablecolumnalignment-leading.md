

- SwiftUI
- TableColumnAlignment
-  leading 

Type Property

# leading

Leading column alignment.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static var leading: TableColumnAlignment { get }
```

## Discussion

With a `layoutDirection` of `leftToRight`, this is equivalent to left; and with a `layoutDirection` of `rightToLeft`, this is equivalent to right.

## See Also

### Getting the alignment

static var automatic: TableColumnAlignment

The default column alignment.

static var center: TableColumnAlignment

Center column alignment.

static var trailing: TableColumnAlignment

Trailing column alignment.

static var numeric: TableColumnAlignment

Column alignment appropriate for numeric content.

static func numeric(Locale.NumberingSystem) -> TableColumnAlignment

Column alignment appropriate for numeric content.

