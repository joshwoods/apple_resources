

- SwiftUI
-  TransitionPhase 

Enumeration

# TransitionPhase

An indication of which the current stage of a transition.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
enum TransitionPhase
```

## Overview

When a view is appearing with a transition, the transition will first be shown with the `willAppear` phase, then will be immediately moved to the `identity` phase. When a view is being removed, its transition is changed from the `identity` phase to the `didDisappear` phase. If a view is removed while it is still transitioning in, then its phase will change to `didDisappear`. If a view is re-added while it is transitioning out, its phase will change back to `identity`.

In the `identity` phase, transitions should generally not make any visual change to the view they are applied to, since the transition’s view modifications in the `identity` phase will be applied to the view as long as it is visible. In the `willAppear` and `didDisappear` phases, transitions should apply a change that will be animated to create the transition. If no animatable change is applied, then the transition will be a no-op.

- See Also: `Transition`

- See Also: `AnyTransition`

## Topics

### Getting the phase

case identity

The transition is being applied to a view that is in the view hierarchy.

case willAppear

The transition is being applied to a view that is about to be inserted into the view hierarchy.

case didDisappear

The transition is being applied to a view that has been requested to be removed from the view hierarchy.

### Getting phase characteristics

var isIdentity: Bool

A Boolean that indicates whether the transition should have an identity effect, i.e. not change the appearance of its view.

var value: Double

A value that can be used to multiply effects that are applied differently depending on the phase.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Defining transitions

func transition(_:)

Associates a transition with the view.

protocol Transition

A description of view changes to apply when a view is added to and removed from the view hierarchy.

struct TransitionProperties

The properties a `Transition` can have.

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

protocol MatchedTransitionSourceConfiguration

A configuration that defines the appearance of a matched transition source.

