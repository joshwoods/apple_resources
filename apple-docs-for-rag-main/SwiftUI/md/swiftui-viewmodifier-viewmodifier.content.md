

- SwiftUI
- ViewModifier
-  ViewModifier.Content 

Type Alias

# ViewModifier.Content

The content view type passed to `body()`.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Content
```

## See Also

### Creating a view modifier

func body(content: Self.Content) -> Self.Body

Gets the current body of the caller.

**Required** Default implementation provided.

associatedtype Body : View

The type of view representing the body.

**Required**

