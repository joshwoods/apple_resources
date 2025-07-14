

- SwiftUI
- SymbolVariants
-  rectangle 

Type Property

# rectangle

A variant that encapsulates the symbol in a rectangle.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let rectangle: SymbolVariants
```

## Discussion

Use this variant with a call to the symbolVariant(_:) modifier to draw symbols in a rectangle, for those symbols that have a rectangle variant:

```
VStack(spacing: 20) {
    HStack(spacing: 20) {
        Image(systemName: "plus")
        Image(systemName: "minus")
        Image(systemName: "xmark")
        Image(systemName: "checkmark")
    }
    HStack(spacing: 20) {
        Image(systemName: "plus")
        Image(systemName: "minus")
        Image(systemName: "xmark")
        Image(systemName: "checkmark")
    }
    .symbolVariant(.rectangle)
}
```

## See Also

### Getting symbol variants

static let none: SymbolVariants

No variant for a symbol.

static let circle: SymbolVariants

A variant that encapsulates the symbol in a circle.

static let square: SymbolVariants

A variant that encapsulates the symbol in a square.

static let fill: SymbolVariants

A variant that fills the symbol.

static let slash: SymbolVariants

A variant that draws a slash through the symbol.

