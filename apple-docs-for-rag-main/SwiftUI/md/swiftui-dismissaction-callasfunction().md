

- SwiftUI
- DismissAction
-  callAsFunction() 

Instance Method

# callAsFunction()

Dismisses the view if it is currently presented.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
func callAsFunction()
```

## Discussion

Don’t call this method directly. SwiftUI calls it for you when you call the DismissAction structure that you get from the Environment:

```
private struct SheetContents: View {
    @Environment(\.dismiss) private var dismiss

    var body: some View {
        Button("Done") {
            dismiss() // Implicitly calls dismiss.callAsFunction()
        }
    }
}
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

