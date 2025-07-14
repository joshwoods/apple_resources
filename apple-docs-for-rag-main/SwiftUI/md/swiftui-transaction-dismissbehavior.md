

- SwiftUI
- Transaction
-  dismissBehavior 

Instance Property

# dismissBehavior

The behavior for how windows will dismiss programmatically when used in conjunction with DismissWindowAction.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var dismissBehavior: DismissBehavior { get set }
```

## Discussion

The default value is `.interactive`.

You can use this property to dismiss windows which may be showing a modal presentation by using the `.destructive` value:

```
struct DismissWindowButton: View {
    @Environment(\.dismissWindow) private var dismissWindow

    var body: some View {
        Button("Close Auxiliary Window") {
            withTransaction(\.dismissBehavior, .destructive) {
                dismissWindow(id: "auxiliary")
            }
        }
    }
}
```

