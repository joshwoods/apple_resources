

- SwiftUI
-  CustomHoverEffect 

Protocol

# CustomHoverEffect

A type that represents how a view should change when a pointer hovers over a view, or when someone looks at the view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
protocol CustomHoverEffect
```

## Overview

Custom hover effects apply their inactive values when the effect is inactive, and their active values when the effect is active. For example, the following effect causes a view to be partially transparent when inactive, but animate to fully opaque when active:

```
struct FadeInHoverEffect: CustomHoverEffect {
    func body(content: Content) -> some CustomHoverEffect {
        content.hoverEffect { effect, isActive, proxy in
            effect.animation(.easeOut) {
                $0.opacity(isActive ? 1 : 0.5)
            }
        }
    }
}
```

This effect can be applied to a view using the `hoverEffect(_:)` modifier:

```
Color.red
    .hoverEffect(FadeInHoverEffect())
```

Hover effects do not affect a view’s layout, and may be applied to a view out-of-process. Therefore an effect’s current phase may not be visible within your app.

## Topics

### Getting built-in hover effects

static var automatic: AutomaticHoverEffect

The default hover effect based on the surrounding context.

static var empty: EmptyHoverEffect

An effect that applies no changes when hovered.

static var highlight: HighlightHoverEffect

A hover effect that highlights views using a light source to indicate position.

static var lift: LiftHoverEffect

A hover effect that slides the pointer under the view and disappears as the view scales up and gains a shadow.

### Creating custom hover effects

func hoverEffect(some CustomHoverEffect, in: HoverEffectGroup?, isEnabled: Bool) -> some CustomHoverEffect

Applies this effect in parallel with the given `effect`.

func hoverEffect(in: HoverEffectGroup?, isEnabled: Bool, body: (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent) -> some CustomHoverEffect

Applies a hover effect based on the current phase.

func hoverEffectGroup(HoverEffectGroup?) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some CustomHoverEffect

Activates this effect as part of an effect group.

func hoverEffectDisabled(Bool) -> some CustomHoverEffect

Disables this hover effect.

### Supporting types

struct AutomaticHoverEffect

The default hover effect based on the surrounding context.

struct EmptyHoverEffect

A base hover effect used to build additional effects.

struct HighlightHoverEffect

A hover effect that highlights views using a light source to indicate position.

struct LiftHoverEffect

A hover effect that slides the pointer under the view and disappears as the view scales up and gains a shadow.

### Associated Types

associatedtype Body : CustomHoverEffect

The type of effect representing the body of this effect. When you create a custom effect, Swift infers this type from your implementation of the required body(content:) method.

**Required**

### Instance Methods

func body(content: Self.Content) -> Self.Body

Defines the effect produced by this effect.

**Required** Default implementation provided.

### Type Aliases

typealias Content

The content effect type passed to `body(content:)`.

## Relationships

### Conforming Types

- AutomaticHoverEffect
- EmptyHoverEffect
- HighlightHoverEffect
- HoverEffect
- LiftHoverEffect
- ModifiedContent

  Conforms when `Content` conforms to `CustomHoverEffect` and `Modifier` conforms to `CustomHoverEffect`.

## See Also

### Changing view appearance for hover events

func hoverEffect(HoverEffect) -> some View

Applies a hover effect to this view.

struct HoverEffect

An effect applied when the pointer hovers over a view.

func hoverEffect(some CustomHoverEffect, in: HoverEffectGroup?, isEnabled: Bool) -> some View

Applies a hover effect to this view, optionally adding it to a HoverEffectGroup.

func hoverEffect(in: HoverEffectGroup?, isEnabled: Bool, body: (EmptyHoverEffectContent, Bool, GeometryProxy) -> some HoverEffectContent) -> some View

Applies a hover effect to this view described by the given closure.

struct HoverEffectGroup

Describes a grouping of effects that activate together.

func hoverEffectGroup() -> some View

Adds an implicit HoverEffectGroup to all effects defined on descendant views, so that all effects added to subviews activate as a group whenever this view or any descendant views are hovered.

func hoverEffectGroup(HoverEffectGroup?) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

protocol HoverEffectContent

A type that describes the effects of a view for a particular hover effect phase.

struct EmptyHoverEffectContent

An empty base effect that you use to build other effects.

func handPointerBehavior(HandPointerBehavior?) -> some View

Sets the behavior of the hand pointer while the user is interacting with the view.

struct HandPointerBehavior

A behavior that can be applied to the hand pointer while the user is interacting with a view.

