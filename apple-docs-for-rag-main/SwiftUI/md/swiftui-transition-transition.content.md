

- SwiftUI
- Transition
-  Transition.Content 

Type Alias

# Transition.Content

The content view type passed to `body()`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
typealias Content = PlaceholderContentView
```

## See Also

### Creating a custom transition

func body(content: Self.Content, phase: TransitionPhase) -> Self.Body

Gets the current body of the caller.

**Required**

associatedtype Body : View

The type of view representing the body.

**Required**

