

- SwiftUI
- AnyTransition
-  asymmetric(insertion:removal:) 

Type Method

# asymmetric(insertion:removal:)

Provides a composite transition that uses a different transition for insertion versus removal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func asymmetric(
    insertion: AnyTransition,
    removal: AnyTransition
) -> AnyTransition
```

## See Also

### Combining and configuring transitions

func animation(Animation?) -> AnyTransition

Attaches an animation to this transition.

func combined(with: AnyTransition) -> AnyTransition

Combines this transition with another, returning a new transition that is the result of both transitions being applied.

