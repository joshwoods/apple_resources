

- SwiftUI
- DismissSearchAction
-  callAsFunction() 

Instance Method

# callAsFunction()

Dismisses the current search operation, if any.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
func callAsFunction()
```

## Discussion

Don’t call this method directly. SwiftUI calls it for you when you call the DismissSearchAction structure that you get from the Environment:

```
struct SearchedView: View {
    @Environment(\.dismissSearch) private var dismissSearch

    var body: some View {
        Button("Cancel") {
            dismissSearch() // Implicitly calls dismissSearch.callAsFunction()
        }
    }
}
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

