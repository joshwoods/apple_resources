

- SwiftUI
- Transition
-  body(content:phase:) 

Instance Method

# body(content:phase:)

Gets the current body of the caller.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@ViewBuilder @MainActor @preconcurrency
func body(
    content: Self.Content,
    phase: TransitionPhase
) -> Self.Body
```

**Required**

## Discussion

`content` is a proxy for the view that will have the modifier represented by `Self` applied to it.

## See Also

### Creating a custom transition

associatedtype Body : View

The type of view representing the body.

**Required**

typealias Content

The content view type passed to `body()`.

