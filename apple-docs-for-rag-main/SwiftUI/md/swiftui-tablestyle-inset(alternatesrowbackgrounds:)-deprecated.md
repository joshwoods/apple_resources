

- SwiftUI
- TableStyle
-  inset(alternatesRowBackgrounds:) Deprecated

Type Method

# inset(alternatesRowBackgrounds:)

The table style that describes the behavior and appearance of a table with its content and selection inset from the table edges.

macOS 12.0–15.4Deprecated

``` source
@MainActor @preconcurrency
static func inset(alternatesRowBackgrounds: Bool) -> InsetTableStyle
```

Available when `Self` is `InsetTableStyle`.

Deprecated

Use the inset style and add the alternatingRowBackgrounds(_:) view modifier instead.

## Parameters 

`alternatesRowBackgrounds`  

Whether the rows should alternate their backgrounds to help visually distinguish them from each other.

## See Also

### Deprecated styles

static func bordered(alternatesRowBackgrounds: Bool) -> BorderedTableStyle

The table style that describes the behavior and appearance of a table with standard border.

Deprecated

