

- SwiftUI
- ListStyle
-  bordered(alternatesRowBackgrounds:) Deprecated

Type Method

# bordered(alternatesRowBackgrounds:)

The list style that describes the behavior and appearance of a list with standard border.

macOS 12.0–15.4Deprecated

``` source
static func bordered(alternatesRowBackgrounds: Bool) -> BorderedListStyle
```

Available when `Self` is `BorderedListStyle`.

Deprecated

Use the bordered style and add the alternatingRowBackgrounds(_:) view modifier instead.

## Parameters 

`alternatesRowBackgrounds`  

Whether the rows should alternate their backgrounds to help visually distinguish them from each other.

## Discussion

Bordered lists are expected to be inset from their outer containers, but do not have inset style rows or selection.

## See Also

### Deprecated styles

static func inset(alternatesRowBackgrounds: Bool) -> InsetListStyle

The list style that describes the behavior and appearance of an inset list with optional alternating row backgrounds.

Deprecated

