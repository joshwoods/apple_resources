

- SwiftData
- Query
-  init(filter:sort:animation:) 

Initializer

# init(filter:sort:animation:)

Create a query with a predicate, and a list of sort descriptors.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    filter: Predicate? = nil,
    sort descriptors: [SortDescriptor] = [],
    animation: Animation
) where Result == [Element]
```

## Parameters 

`filter`  

A predicate on `Element`

`descriptors`  

Sort orders for the result.

`animation`  

The animation to use for user interface changes that result from changes to the fetched results.

## Discussion

Use `Query` within a view by wrapping the variable for the query’s result:

```
struct RecipeList: View {
    // Favorite recipes sorted by date of creation
    @Query(
        filter: #Predicate { $0.isFavorite == true },
        sort: [SortDescriptor(\.dateCreated)]
    )
    var favoriteRecipes: [Recipe]

    var body: some View {
        List(favoriteRecipes) { RecipeDetails($0) }
    }
}
```

## See Also

### Creating a query

init(FetchDescriptor&lt;Element>, animation: Animation)

Create a query with a SwiftData fetch descriptor.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, animation: Animation)

Creates a query with a predicate, a key path to a property for sorting, and the order to sort by.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, animation: Animation)

Creates a query with a predicate, a key path to a property for sorting, and the order to sort by.

init(FetchDescriptor&lt;Element>, transaction: Transaction?)

Create a query with a SwiftData fetch descriptor.

init(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], transaction: Transaction?)

Create a query with a predicate, and a list of sort descriptors.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, transaction: Transaction?)

Create a query with a predicate, a key path to a property for sorting, and the order to sort by.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, transaction: Transaction?)

Create a query with a predicate, a key path to a property for sorting, and the order to sort by.

