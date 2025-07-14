

- SwiftData
- Query
-  init(filter:sort:order:transaction:) 

Initializer

# init(filter:sort:order:transaction:)

Create a query with a predicate, a key path to a property for sorting, and the order to sort by.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    filter: Predicate? = nil,
    sort keyPath: KeyPath,
    order: SortOrder = .forward,
    transaction: Transaction? = nil
) where Result == [Element], Value : Comparable
```

## Parameters 

`filter`  

A predicate on `Element`

`sort`  

Key path to property used for sorting.

`order`  

Whether to sort in forward or reverse order.

`transaction`  

A transaction to use for user interface changes that result from changes to the fetched results.

## Discussion

Use `Query` within a view by wrapping the variable for the query’s result:

```
struct RecipeList: View {
    // Recipes sorted by date of creation
    @Query(sort: \.dateCreated)
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

init(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], animation: Animation)

Create a query with a predicate, and a list of sort descriptors.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, animation: Animation)

Creates a query with a predicate, a key path to a property for sorting, and the order to sort by.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value>, order: SortOrder, animation: Animation)

Creates a query with a predicate, a key path to a property for sorting, and the order to sort by.

init(FetchDescriptor&lt;Element>, transaction: Transaction?)

Create a query with a SwiftData fetch descriptor.

init(filter: Predicate&lt;Element>?, sort: [SortDescriptor&lt;Element>], transaction: Transaction?)

Create a query with a predicate, and a list of sort descriptors.

init&lt;Value>(filter: Predicate&lt;Element>?, sort: KeyPath&lt;Element, Value?>, order: SortOrder, transaction: Transaction?)

Create a query with a predicate, a key path to a property for sorting, and the order to sort by.

