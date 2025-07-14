

- SwiftUI
-  SymbolVariants 

Structure

# SymbolVariants

A variant of a symbol.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SymbolVariants
```

## Overview

Many of the SF Symbols that you can add to your app using an Image or a Label instance have common variants, like a filled version or a version that’s contained within a circle. The symbol’s name indicates the variant:

```
VStack(alignment: .leading) {
    Label("Default", systemImage: "heart")
    Label("Fill", systemImage: "heart.fill")
    Label("Circle", systemImage: "heart.circle")
    Label("Circle Fill", systemImage: "heart.circle.fill")
}
```

You can configure a part of your view hierarchy to use a particular variant for all symbols in that view and its child views using `SymbolVariants`. Add the symbolVariant(_:) modifier to a view to set a variant for that view’s environment. For example, you can use the modifier to create the same set of labels as in the example above, using only the base name of the symbol in the label declarations:

```
VStack(alignment: .leading) {
    Label("Default", systemImage: "heart")
    Label("Fill", systemImage: "heart")
        .symbolVariant(.fill)
    Label("Circle", systemImage: "heart")
        .symbolVariant(.circle)
    Label("Circle Fill", systemImage: "heart")
        .symbolVariant(.circle.fill)
}
```

Alternatively, you can set the variant in the environment directly by passing the symbolVariants environment value to the environment(_:_:) modifier:

```
Label("Fill", systemImage: "heart")
    .environment(\.symbolVariants, .fill)
```

SwiftUI sets a variant for you in some environments. For example, SwiftUI automatically applies the fill symbol variant for items that appear in the `content` closure of the swipeActions(edge:allowsFullSwipe:content:) method, or as the tab bar items of a TabView.

## Topics

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

static let slash: SymbolVariants

A variant that draws a slash through the symbol.

### Modifying a variant

var circle: SymbolVariants

A version of the variant that’s encapsulated in a circle.

var square: SymbolVariants

A version of the variant that’s encapsulated in a square.

var rectangle: SymbolVariants

A version of the variant that’s encapsulated in a rectangle.

var fill: SymbolVariants

A filled version of the variant.

var slash: SymbolVariants

A slashed version of the variant.

### Comparing variants

func contains(SymbolVariants) -> Bool

Returns a Boolean value that indicates whether the current variant contains the specified variant.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Setting a symbol variant

func symbolVariant(SymbolVariants) -> some View

Makes symbols within the view show a particular variant.

var symbolVariants: SymbolVariants

The symbol variant to use in this environment.

