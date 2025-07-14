

- Assignables
- AssignedWorkDocumentView
-  body 

Instance Property

# body

The content and behavior of the view.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@MainActor @preconcurrency
var body: some View { get }
```

## Discussion

When you implement a custom view, you must implement a computed `body` property to provide the content for your view. Return a view that’s composed of built-in views that SwiftUI provides, plus other composite views that you’ve already defined:

```
struct MyView: View {
    var body: some View {
        Text("Hello, World!")
    }
}
```

For more information about composing views and a view hierarchy, see doc:Declaring-a-Custom-View.

## See Also

### Implementing a view

typealias Document

The document type that this view presents.

