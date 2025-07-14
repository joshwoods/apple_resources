

- SwiftUI
- Transition
-  properties 

Type Property

# properties

Returns the properties this transition type has.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
static var properties: TransitionProperties { get }
```

**Required** Default implementation provided.

## Discussion

Defaults to `TransitionProperties()`.

## Default Implementations

### Transition Implementations

static var properties: TransitionProperties

Returns the properties this transition type has.

## See Also

### Configuring a transition

func animation(Animation?) -> some Transition

Attaches an animation to this transition.

