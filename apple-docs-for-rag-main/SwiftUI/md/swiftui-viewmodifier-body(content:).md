

- SwiftUI
- ViewModifier
-  body(content:) 

Instance Method

# body(content:)

Gets the current body of the caller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func body(content: Self.Content) -> Self.Body
```

**Required** Default implementation provided.

## Discussion

`content` is a proxy for the view that will have the modifier represented by `Self` applied to it.

## Default Implementations

### ViewModifier Implementations

func body(content: Self.Content) -> Self.Body

Gets the current body of the caller.

## See Also

### Creating a view modifier

associatedtype Body : View

The type of view representing the body.

**Required**

typealias Content

The content view type passed to `body()`.

