

- SwiftUI
-  AsymmetricTransition 

Structure

# AsymmetricTransition

A composite `Transition` that uses a different transition for insertion versus removal.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
struct AsymmetricTransition where Insertion : Transition, Removal : Transition
```

## Topics

### Creating the transition

init(insertion: Insertion, removal: Removal)

Creates a composite `Transition` that uses a different transition for insertion versus removal.

### Getting transition properties

var insertion: Insertion

The `Transition` defining the insertion phase of `self`.

var removal: Removal

The `Transition` defining the removal phase of `self`.

## Relationships

### Conforms To

- Transition

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

