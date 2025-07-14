

- SwiftUI
- RefreshAction
-  callAsFunction() 

Instance Method

# callAsFunction()

Initiates a refresh action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func callAsFunction() async
```

## Discussion

Don’t call this method directly. SwiftUI calls it when you call the RefreshAction structure that you get from the Environment:

```
struct RefreshableView: View {
    @Environment(\.refresh) private var refresh

    var body: some View {
        Button("Refresh") {
            Task {
                await refresh?()  // Implicitly calls refresh.callAsFunction()
            }
        }
        .disabled(refresh == nil)
    }
}
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*. For information about asynchronous operations in Swift, see Concurrency.

