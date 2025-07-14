

- FamilyControls
- FamilyActivityPicker
-  body 

Instance Property

# body

The content and behavior of the view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

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

### Accessing the Content

typealias Body

The type of view representing the body of this view.

