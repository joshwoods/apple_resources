

- SwiftUI
- AnyTransition
-  combined(with:) 

Instance Method

# combined(with:)

Combines this transition with another, returning a new transition that is the result of both transitions being applied.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func combined(with other: AnyTransition) -> AnyTransition
```

## See Also

### Combining and configuring transitions

func animation(Animation?) -> AnyTransition

Attaches an animation to this transition.

static func asymmetric(insertion: AnyTransition, removal: AnyTransition) -> AnyTransition

Provides a composite transition that uses a different transition for insertion versus removal.

