

- SwiftUI
- TableStyle
-  inset 

Type Property

# inset

The table style that describes the behavior and appearance of a table with its content and selection inset from the table edges.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var inset: InsetTableStyle { get }
```

Available when `Self` is `InsetTableStyle`.

## Discussion

To customize whether the rows of the table should alternate their backgrounds, use alternatingRowBackgrounds(_:).

## See Also

### Getting built-in table styles

static var automatic: AutomaticTableStyle

The default table style in the current context.

static var bordered: BorderedTableStyle

The table style that describes the behavior and appearance of a table with standard border.

