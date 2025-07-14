

- SwiftUI
- View
-  searchScopes(\_:scopes:) 

Instance Method

# searchScopes(\_:scopes:)

Configures the search scopes for this view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.4+visionOS 1.0+

``` source
nonisolated
func searchScopes(
    _ scope: Binding,
    @ViewBuilder scopes: () -> S
) -> some View where V : Hashable, S : View
```

## Parameters 

`scope`  

The active scope of the search field.

`scopes`  

A view builder that represents the scoping options SwiftUI uses to populate a Picker.

## Mentioned in 

Scoping a search operation

## Discussion

To enable people to narrow the scope of their searches, you can create a type that represents the possible scopes, and then create a state variable to hold the current selection. For example, you can scope the product search to just fruits or just vegetables:

```
enum ProductScope {
    case fruit
    case vegetable
}

@State private var scope: ProductScope = .fruit
```

Provide a binding to the scope, as well as a view that represents each scope:

```
ProductList()
    .searchable(text: $text, tokens: $tokens) { token in
        switch token {
        case .apple: Text("Apple")
        case .pear: Text("Pear")
        case .banana: Text("Banana")
        }
    }
    .searchScopes($scope) {
        Text("Fruit").tag(ProductScope.fruit)
        Text("Vegetable").tag(ProductScope.vegetable)
    }
```

SwiftUI uses this binding and view to add a Picker with the search field. In iOS, iPadOS, macOS, and tvOS, the picker appears below the search field when search is active. To ensure that the picker operates correctly, match the type of the scope binding with the type of each view’s tag. Then modify your search to account for the current value of the `scope` state property.

For more information about using searchable modifiers, see Adding a search interface to your app.

## See Also

### Limiting search scope

Scoping a search operation

Divide the search space into a few broad categories.

func searchScopes&lt;V, S>(Binding&lt;V>, activation: SearchScopeActivation, () -> S) -> some View

Configures the search scopes for this view with the specified activation strategy.

struct SearchScopeActivation

The ways that searchable modifiers can show or hide search scopes.

