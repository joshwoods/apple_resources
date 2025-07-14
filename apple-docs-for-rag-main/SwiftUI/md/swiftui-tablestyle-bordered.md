

- SwiftUI
- TableStyle
-  bordered 

Type Property

# bordered

The table style that describes the behavior and appearance of a table with standard border.

macOS 12.0+

``` source
@MainActor @preconcurrency
static var bordered: BorderedTableStyle { get }
```

Available when `Self` is `BorderedTableStyle`.

## Discussion

Bordered tables are expected to be inset from their outer containers, but do not have inset style rows or selection.

To customize whether the rows of the table should alternate their backgrounds, use alternatingRowBackgrounds(_:).

## See Also

### Getting built-in table styles

static var automatic: AutomaticTableStyle

The default table style in the current context.

static var inset: InsetTableStyle

The table style that describes the behavior and appearance of a table with its content and selection inset from the table edges.

