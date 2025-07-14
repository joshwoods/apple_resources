

- SwiftUI
- PaletteSelectionEffect
-  automatic 

Type Property

# automatic

Applies the system’s default effect when selected.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
static let automatic: PaletteSelectionEffect
```

## Discussion

When using un-tinted SF Symbols or template images, the current tint color is applied to the selected items’ image. If the provided SF Symbols have custom tints, a stroke is drawn around selected items.

## See Also

### Getting palette selection effects

static let custom: PaletteSelectionEffect

Does not apply any system effect when selected.

static func symbolVariant(SymbolVariants) -> PaletteSelectionEffect

Applies the specified symbol variant when selected.

