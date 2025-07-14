

- SwiftUI
- Search
-  Scoping a search operation 

Article

# Scoping a search operation

Divide the search space into a few broad categories.

## Overview

If the data you want to search falls into a few categories, you can define different scopes to help people narrow their search. When you define a scope, SwiftUI presents a picker that people can use to choose one of them. You then use the current scope selection as one of the inputs to the search operation.

### Define the possible scopes

Start by creating a type that conforms to the Hashable protocol to represent the possible scopes. For example, you can use an enumeration to scope a product search to just fruits or just vegetables:

```
enum ProductScope {
    case fruit
    case vegetable
}
```

Then create a property to store the current scope, either as a state variable in a view, or a published property in your model:

```
@Published var scope: ProductScope = .fruit
```

### Apply the scope

To use the scope information, bind the current scope to the searchScopes(_:scopes:) modifier. You also indicate a set of views that correspond to the different scopes. Like the searchSuggestions(_:) modifier, the scopes modifier operates on the searchable modifier that’s closer to the modified view, so it needs to follow the searchable modifier:

```
ProductList(departmentId: departmentId, productId: $productId)
    .searchable(text: $model.searchText, tokens: $model.tokens) { token in
        switch token {
        case .apple: Text("Apple")
        case .pear: Text("Pear")
        case .banana: Text("Banana")
        }
    }
    .searchScopes($model.scope) {
        Text("Fruit").tag(ProductScope.fruit)
        Text("Vegetable").tag(ProductScope.vegetable)
    }
```

SwiftUI uses the binding and views to add a Picker to the search field. By default, the picker appears below the search field in macOS when search is active, or in iOS when someone starts entering text into the search field:

- macOS
- iOS

You can change when the picker appears by using the searchScopes(_:activation:_:) modifier instead, and supplying one of the SearchScopeActivation values, like onTextEntry or onSearchPresentation.

To ensure that the picker operates correctly, match the type of the scope binding with the type of each view’s tag. In the above example, both the `scope` input and the tags for each view have the type `ProductScope`.

### Use the scope in your search

Modify your search to account for the current value of the `scope` property, if you offer it, along with the text and tokens in the query. For example, you might include the scope as one element of a predicate that you define for a Core Data fetch request. For more information about conducting a search, see Performing a search operation.

## See Also

### Limiting search scope

func searchScopes&lt;V, S>(Binding&lt;V>, scopes: () -> S) -> some View

Configures the search scopes for this view.

func searchScopes&lt;V, S>(Binding&lt;V>, activation: SearchScopeActivation, () -> S) -> some View

Configures the search scopes for this view with the specified activation strategy.

struct SearchScopeActivation

The ways that searchable modifiers can show or hide search scopes.

