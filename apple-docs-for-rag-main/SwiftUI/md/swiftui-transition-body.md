

- SwiftUI
- Transition
-  Body 

Associated Type

# Body

The type of view representing the body.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
associatedtype Body : View
```

**Required**

## See Also

### Creating a custom transition

func body(content: Self.Content, phase: TransitionPhase) -> Self.Body

Gets the current body of the caller.

**Required**

typealias Content

The content view type passed to `body()`.

