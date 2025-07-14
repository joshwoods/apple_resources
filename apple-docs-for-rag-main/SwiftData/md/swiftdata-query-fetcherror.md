

- SwiftData
- Query
-  fetchError 

Instance Property

# fetchError

An error encountered during the most recent attempt to fetch data.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
var fetchError: (any Error)? { get }
```

## Discussion

This value is `nil` unless an fetch attempt failed. It contains the latest error from SwiftData. Access it from Query’s stored property:

```
struct RecipeList: View {
    @Query var recipes: [Recipe]
    var body: some View {
        ErrorIndicatorView(_recipes.fetchError)
    }
}
```

Note

Only access this property within of a view’s `body` property, otherwise its value may be invalid.

Note

When an fetch error occurs, `wrappedValue` retains results from the last successful fetch. Its value will update once a new fetch succeeds.

## See Also

### Getting query configuration

var modelContext: ModelContext

Current model context `Query` interacts with.

