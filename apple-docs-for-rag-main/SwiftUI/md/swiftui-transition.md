

- SwiftUI
-  Transition 

Protocol

# Transition

A description of view changes to apply when a view is added to and removed from the view hierarchy.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
protocol Transition
```

## Overview

A transition should generally be made by applying one or more modifiers to the `content`. For symmetric transitions, the `isIdentity` property on `phase` can be used to change the properties of modifiers. For asymmetric transitions, the phase itself can be used to change those properties. Transitions should not use any identity-affecting changes like `.id`, `if`, and `switch` on the `content`, since doing so would reset the state of the view they’re applied to, causing wasted work and potentially surprising behavior when it appears and disappears.

The following code defines a transition that can be used to change the opacity and rotation when a view appears and disappears.

```
struct RotatingFadeTransition: Transition {
    func body(content: Content, phase: TransitionPhase) -> some View {
        content
          .opacity(phase.isIdentity ? 1.0 : 0.0)
          .rotationEffect(phase.rotation)
    }
}
extension TransitionPhase {
    fileprivate var rotation: Angle {
        switch self {
        case .willAppear: return .degrees(30)
        case .identity: return .zero
        case .didDisappear: return .degrees(-30)
        }
    }
}
```

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

- See Also: `TransitionPhase`

- See Also: `AnyTransition`

## Topics

### Getting built-in transitions

static var blurReplace: BlurReplaceTransition

A transition that animates the insertion or removal of a view by combining blurring and scaling effects.

static func blurReplace(BlurReplaceTransition.Configuration) -> Self

A transition that animates the insertion or removal of a view by combining blurring and scaling effects.

static var identity: IdentityTransition

A transition that returns the input view, unmodified, as the output view.

static func move(edge: Edge) -> Self

Returns a transition that moves the view away, towards the specified edge of the view.

static func offset(CGSize) -> Self

Returns a transition that offset the view by the specified amount.

static func offset(x: CGFloat, y: CGFloat) -> Self

Returns a transition that offset the view by the specified x and y values.

static var opacity: OpacityTransition

A transition from transparent to opaque on insertion, and from opaque to transparent on removal.

static func push(from: Edge) -> Self

Creates a transition that when added to a view will animate the view’s insertion by moving it in from the specified edge while fading it in, and animate its removal by moving it out towards the opposite edge and fading it out.

static var scale: ScaleTransition

Returns a transition that scales the view.

static func scale(Double, anchor: UnitPoint) -> Self

Returns a transition that scales the view by the specified amount.

static var slide: SlideTransition

A transition that inserts by moving in from the leading edge, and removes by moving out towards the trailing edge.

static var symbolEffect: SymbolEffectTransition

A transition that applies the default symbol effect transition to symbol images within the inserted or removed view hierarchy. Other views are unaffected by this transition.

static func symbolEffect&lt;T>(T, options: SymbolEffectOptions) -> SymbolEffectTransition

Creates a transition that applies the provided effect to symbol images within the inserted or removed view hierarchy. Other views are unaffected by this transition.

### Configuring a transition

func animation(Animation?) -> some Transition

Attaches an animation to this transition.

static var properties: TransitionProperties

Returns the properties this transition type has.

**Required** Default implementation provided.

### Using a transition

func apply&lt;V>(content: V, phase: TransitionPhase) -> some View

func combined&lt;T>(with: T) -> some Transition

### Creating a custom transition

func body(content: Self.Content, phase: TransitionPhase) -> Self.Body

Gets the current body of the caller.

**Required**

associatedtype Body : View

The type of view representing the body.

**Required**

typealias Content

The content view type passed to `body()`.

### Supporting types

struct BlurReplaceTransition

A transition that animates the insertion or removal of a view by combining blurring and scaling effects.

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

## Relationships

### Conforming Types

- AsymmetricTransition
- BlurReplaceTransition
- IdentityTransition
- MoveTransition
- OffsetTransition
- OpacityTransition
- PushTransition
- ScaleTransition
- SlideTransition
- SymbolEffectTransition

## See Also

### Defining transitions

func transition(_:)

Associates a transition with the view.

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

