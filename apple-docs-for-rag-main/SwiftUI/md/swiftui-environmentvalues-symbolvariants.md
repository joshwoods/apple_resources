

- SwiftUI
- EnvironmentValues
-  symbolVariants 

Instance Property

# symbolVariants

The symbol variant to use in this environment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var symbolVariants: SymbolVariants { get set }
```

## Discussion

You set this environment value indirectly by using the symbolVariant(_:) view modifier. However, you access the environment variable directly using the environment(_:_:) modifier. Do this when you want to use the none variant to ignore the value that’s already in the environment:

```
HStack {
    Image(systemName: "heart")
    Image(systemName: "heart")
        .environment(\.symbolVariants, .none)
}
.symbolVariant(.fill)
```

## See Also

### Setting a symbol variant

func symbolVariant(SymbolVariants) -> some View

Makes symbols within the view show a particular variant.

struct SymbolVariants

A variant of a symbol.

