

- SwiftUI
-  MatchedTransitionSourceConfiguration 

Protocol

# MatchedTransitionSourceConfiguration

A configuration that defines the appearance of a matched transition source.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol MatchedTransitionSourceConfiguration : Sendable
```

## Topics

### Instance Methods

func background(Color) -> some MatchedTransitionSourceConfiguration

Specifies a color that will be drawn behind the content within the matched transition source.

func clipShape(RoundedRectangle) -> some MatchedTransitionSourceConfiguration

Applies the specified shape as to the matched transition source, clipping its content.

func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat) -> some MatchedTransitionSourceConfiguration

Applies the specified shadow effect to the matched transition source.

## Relationships

### Inherits From

- Sendable

### Conforming Types

- EmptyMatchedTransitionSourceConfiguration

## See Also

### Defining transitions

func transition(_:)

Associates a transition with the view.

protocol Transition

A description of view changes to apply when a view is added to and removed from the view hierarchy.

struct TransitionProperties

The properties a `Transition` can have.

enum TransitionPhase

An indication of which the current stage of a transition.

struct AsymmetricTransition

A composite `Transition` that uses a different transition for insertion versus removal.

struct AnyTransition

A type-erased transition.

func contentTransition(ContentTransition) -> some View

Modifies the view to use a given transition as its method of animating changes to the contents of its views.

var contentTransition: ContentTransition

The current method of animating the contents of views.

var contentTransitionAddsDrawingGroup: Bool

A Boolean value that controls whether views that render content transitions use GPU-accelerated rendering.

struct ContentTransition

A kind of transition that applies to the content within a single view, rather than to the insertion or removal of a view.

struct PlaceholderContentView

A placeholder used to construct an inline modifier, transition, or other helper type.

func navigationTransition(some NavigationTransition) -> some View

Sets the navigation transition style for this view.

protocol NavigationTransition

A type that defines the transition to use when navigating to a view.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

func matchedTransitionSource(id: some Hashable, in: Namespace.ID, configuration: (EmptyMatchedTransitionSourceConfiguration) -> some MatchedTransitionSourceConfiguration) -> some View

Identifies this view as the source of a navigation transition, such as a zoom transition.

