

- SwiftUI
- View
-  Body 

Associated Type

# Body

The type of view representing the body of this view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype Body : View
```

**Required**

## Discussion

When you create a custom view, Swift infers this type from your implementation of the required body property.

## See Also

### Implementing a custom view

var body: Self.Body

The content and behavior of the view.

**Required** Default implementations provided.

func modifier&lt;T>(T) -> ModifiedContent&lt;Self, T>

Applies a modifier to a view and returns a new view.

Previews in Xcode

Generate dynamic, interactive previews of your custom views.

