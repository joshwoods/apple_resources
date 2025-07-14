

- SwiftUI
- SymbolVariants
-  none 

Type Property

# none

No variant for a symbol.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let none: SymbolVariants
```

## Discussion

Using this variant with the symbolVariant(_:) modifier doesn’t have any effect. Instead, to show a symbol that ignores the current variant, directly set the symbolVariants environment value to `none` using the environment(_:_:) modifer:

```
HStack {
    Image(systemName: "heart")
    Image(systemName: "heart")
        .environment(\.symbolVariants, .none)
}
.symbolVariant(.fill)
```

## See Also

### Getting symbol variants

static let circle: SymbolVariants

A variant that encapsulates the symbol in a circle.

static let square: SymbolVariants

A variant that encapsulates the symbol in a square.

static let rectangle: SymbolVariants

A variant that encapsulates the symbol in a rectangle.

static let fill: SymbolVariants

A variant that fills the symbol.

static let slash: SymbolVariants

A variant that draws a slash through the symbol.

