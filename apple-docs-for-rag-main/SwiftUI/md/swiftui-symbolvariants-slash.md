

- SwiftUI
- SymbolVariants
-  slash 

Type Property

# slash

A variant that draws a slash through the symbol.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let slash: SymbolVariants
```

## Discussion

Use this variant with a call to the symbolVariant(_:) modifier to draw symbols with a slash, for those symbols that have such a variant:

```
VStack(spacing: 20) {
    HStack(spacing: 20) {
        Image(systemName: "flag")
        Image(systemName: "heart")
        Image(systemName: "bolt")
        Image(systemName: "star")
    }
    HStack(spacing: 20) {
        Image(systemName: "flag")
        Image(systemName: "heart")
        Image(systemName: "bolt")
        Image(systemName: "star")
    }
    .symbolVariant(.slash)
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

static let rectangle: SymbolVariants

A variant that encapsulates the symbol in a rectangle.

static let fill: SymbolVariants

A variant that fills the symbol.

