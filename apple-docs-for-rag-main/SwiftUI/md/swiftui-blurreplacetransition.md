

- SwiftUI
-  BlurReplaceTransition 

Structure

# BlurReplaceTransition

A transition that animates the insertion or removal of a view by combining blurring and scaling effects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
struct BlurReplaceTransition
```

## Topics

### Creating the transition

init(configuration: BlurReplaceTransition.Configuration)

Creates a new transition.

var configuration: BlurReplaceTransition.Configuration

The transition configuration.

struct Configuration

Configuration properties for a transition.

## Relationships

### Conforms To

- Transition

## See Also

### Supporting types

struct IdentityTransition

A transition that returns the input view, unmodified, as the output view.

struct MoveTransition

Returns a transition that moves the view away, towards the specified edge of the view.

struct OffsetTransition

Returns a transition that offset the view by the specified amount.

struct OpacityTransition

A transition from transparent to opaque on insertion, and from opaque to transparent on removal.

struct PushTransition

A transition that when added to a view will animate the view’s insertion by moving it in from the specified edge while fading it in, and animate its removal by moving it out towards the opposite edge and fading it out.

struct ScaleTransition

Returns a transition that scales the view.

struct SlideTransition

A transition that inserts by moving in from the leading edge, and removes by moving out towards the trailing edge.

