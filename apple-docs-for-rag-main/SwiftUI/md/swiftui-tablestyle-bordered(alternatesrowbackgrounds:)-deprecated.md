

- SwiftUI
- TableStyle
-  bordered(alternatesRowBackgrounds:) Deprecated

Type Method

# bordered(alternatesRowBackgrounds:)

The table style that describes the behavior and appearance of a table with standard border.

macOS 12.0–15.4Deprecated

``` source
@MainActor @preconcurrency
static func bordered(alternatesRowBackgrounds: Bool) -> BorderedTableStyle
```

Available when `Self` is `BorderedTableStyle`.

Deprecated

Use the bordered style and add the alternatingRowBackgrounds(_:) view modifier instead.

## Parameters 

`alternatesRowBackgrounds`  

Whether the rows should alternate their backgrounds to help visually distinguish them from each other.

## Discussion

Bordered tables are expected to be inset from their outer containers, but do not have inset style rows or selection.

## See Also

### Deprecated styles

static func inset(alternatesRowBackgrounds: Bool) -> InsetTableStyle

The table style that describes the behavior and appearance of a table with its content and selection inset from the table edges.

Deprecated

