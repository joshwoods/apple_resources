

- SwiftUI
- PaletteSelectionEffect
-  custom 

Type Property

# custom

Does not apply any system effect when selected.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static let custom: PaletteSelectionEffect
```

## Discussion

Note

Make sure to manually implement a way to indicate selection when using this case. For example, you could dynamically resolve the item’s image based on the selection state.

## See Also

### Getting palette selection effects

static let automatic: PaletteSelectionEffect

Applies the system’s default effect when selected.

static func symbolVariant(SymbolVariants) -> PaletteSelectionEffect

Applies the specified symbol variant when selected.

