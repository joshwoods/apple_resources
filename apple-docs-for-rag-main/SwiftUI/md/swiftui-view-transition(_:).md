

- SwiftUI
- View
-  transition(\_:) 

Instance Method

# transition(\_:)

Associates a transition with the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func transition(_ t: AnyTransition) -> some View
```

Show all declarations

## Discussion

When this view appears or disappears, the transition will be applied to it, allowing for animating it in and out.

The following code will conditionally show MyView, and when it appears or disappears, will use a slide transition to show it.

```
if isActive {
    MyView()
        .transition(.slide)
}
Button("Toggle") {
    withAnimation {
        isActive.toggle()
    }
}
```

## See Also

### Defining transitions

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

protocol MatchedTransitionSourceConfiguration

A configuration that defines the appearance of a matched transition source.

