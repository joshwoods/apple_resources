

- SwiftUI
- View
-  symbolVariant(\_:) 

Instance Method

# symbolVariant(\_:)

Makes symbols within the view show a particular variant.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func symbolVariant(_ variant: SymbolVariants) -> some View
```

## Parameters 

`variant`  

The variant to use for symbols. Use the values in SymbolVariants.

## Return Value

A view that applies the specified symbol variant or variants to itself and its child views.

## Discussion

When you want all the SF Symbols in a part of your app’s user interface to use the same variant, use the `symbolVariant(_:)` modifier with a SymbolVariants value, like fill:

```
VStack(spacing: 20) {
    HStack(spacing: 20) {
        Image(systemName: "person")
        Image(systemName: "folder")
        Image(systemName: "gearshape")
        Image(systemName: "list.bullet")
    }

    HStack(spacing: 20) {
        Image(systemName: "person")
        Image(systemName: "folder")
        Image(systemName: "gearshape")
        Image(systemName: "list.bullet")
    }
    .symbolVariant(.fill) // Shows filled variants, when available.
}
```

A symbol that doesn’t have the specified variant remains unaffected. In the example above, the `list.bullet` symbol doesn’t have a filled variant, so the `symbolVariant(_:)` modifer has no effect.

If you apply the modifier more than once, its effects accumulate. Alternatively, you can apply multiple variants in one call:

```
Label("Airplane", systemImage: "airplane.circle.fill")

Label("Airplane", systemImage: "airplane")
    .symbolVariant(.circle)
    .symbolVariant(.fill)

Label("Airplane", systemImage: "airplane")
    .symbolVariant(.circle.fill)
```

All of the labels in the code above produce the same output:

You can apply all these variants in any order, but if you apply more than one shape variant, the one closest to the symbol takes precedence. For example, the following image uses the square shape:

```
Image(systemName: "arrow.left")
    .symbolVariant(.square) // This shape takes precedence.
    .symbolVariant(.circle)
    .symbolVariant(.fill)
```

To cause a symbol to ignore the variants currently in the environment, directly set the symbolVariants environment value to none using the environment(_:_:) modifer.

## See Also

### Setting a symbol variant

var symbolVariants: SymbolVariants

The symbol variant to use in this environment.

struct SymbolVariants

A variant of a symbol.

