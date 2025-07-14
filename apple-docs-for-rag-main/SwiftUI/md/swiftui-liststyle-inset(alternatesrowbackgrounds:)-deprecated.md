

- SwiftUI
- ListStyle
-  inset(alternatesRowBackgrounds:) Deprecated

Type Method

# inset(alternatesRowBackgrounds:)

The list style that describes the behavior and appearance of an inset list with optional alternating row backgrounds.

macOS 12.0–15.4Deprecated

``` source
static func inset(alternatesRowBackgrounds: Bool) -> InsetListStyle
```

Available when `Self` is `InsetListStyle`.

Deprecated

Use the inset style and add the alternatingRowBackgrounds(_:) view modifier instead.

## Parameters 

`alternatesRowBackgrounds`  

Whether the rows should alternate their backgrounds to help visually distinguish them from each other.

## See Also

### Deprecated styles

static func bordered(alternatesRowBackgrounds: Bool) -> BorderedListStyle

The list style that describes the behavior and appearance of a list with standard border.

Deprecated

