

- SwiftUI
- View
-  body 

Instance Property

# body

The content and behavior of the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@ViewBuilder @MainActor @preconcurrency
var body: Self.Body { get }
```

**Required** Default implementations provided.

## Mentioned in 

Declaring a custom view

## Discussion

When you implement a custom view, you must implement a computed `body` property to provide the content for your view. Return a view that’s composed of built-in views that SwiftUI provides, plus other composite views that you’ve already defined:

```
struct MyView: View {
    var body: some View {
        Text("Hello, World!")
    }
}
```

For more information about composing views and a view hierarchy, see Declaring a custom view.

## Default Implementations

### NSViewControllerRepresentable Implementations

var body: Never

Declares the content and behavior of this view.

### NSViewRepresentable Implementations

var body: Never

Declares the content and behavior of this view.

### UIViewControllerRepresentable Implementations

var body: Never

Declares the content and behavior of this view.

### UIViewRepresentable Implementations

var body: Never

Declares the content and behavior of this view.

### View Implementations

var body: _ShapeView&lt;Self, ForegroundStyle>

### WKInterfaceObjectRepresentable Implementations

var body: Never

Declares the content and behavior of this view.

## See Also

### Implementing a custom view

associatedtype Body : View

The type of view representing the body of this view.

**Required**

func modifier&lt;T>(T) -> ModifiedContent&lt;Self, T>

Applies a modifier to a view and returns a new view.

Previews in Xcode

Generate dynamic, interactive previews of your custom views.

