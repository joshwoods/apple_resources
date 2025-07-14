

- SwiftUI
-  HoverEffectContent 

Protocol

# HoverEffectContent

A type that describes the effects of a view for a particular hover effect phase.

visionOS 2.0+

``` source
protocol HoverEffectContent
```

## Overview

```
Color.red
    .hoverEffect { effect, isActive, proxy in
        effect.opacity(isActive ? 1 : 0.5)
    }
```

You don’t conform to this protocol yourself. Instead, effects are described by calling modifier functions on other effects, like the `opacity(_:)` modifier used in the example above.

## Topics

### Instance Methods

func animation(Animation?, body: (EmptyHoverEffectContent) -> some HoverEffectContent) -> some HoverEffectContent

Applies the given Animation to all effects within the `body` closure.

func clipShape&lt;S>(S, style: FillStyle) -> some HoverEffectContent

Sets a clipping shape for the view.

func offset(CGSize) -> some HoverEffectContent

Offsets the view by the horizontal and vertical amount specified in the offset parameter.

func offset(x: CGFloat, y: CGFloat) -> some HoverEffectContent

Offsets the view by the specified horizontal and vertical distances.

func opacity(Double) -> some HoverEffectContent

Sets the transparency of the view.

func rotationEffect(Angle, anchor: UnitPoint) -> some HoverEffectContent

Rotates content in two dimensions around the specified point.

func scaleEffect(_:anchor:)

Scales the view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> some HoverEffectContent

Scales the view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

func transformEffect(CGAffineTransform) -> some HoverEffectContent

Applies an affine transformation to the view’s rendered output.

## Relationships

### Conforming Types

- EmptyHoverEffectContent
- ModifiedContent

  Conforms when `Content` conforms to `HoverEffectContent` and `Modifier` conforms to `HoverEffectContent`.

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

protocol CustomHoverEffect

A type that represents how a view should change when a pointer hovers over a view, or when someone looks at the view.

struct HoverEffectGroup

Describes a grouping of effects that activate together.

func hoverEffectGroup() -> some View

Adds an implicit HoverEffectGroup to all effects defined on descendant views, so that all effects added to subviews activate as a group whenever this view or any descendant views are hovered.

func hoverEffectGroup(HoverEffectGroup?) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

func hoverEffectGroup(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior) -> some View

Adds a HoverEffectGroup to all effects defined on descendant views, and activates the group whenever this view or any descendant views are hovered.

struct EmptyHoverEffectContent

An empty base effect that you use to build other effects.

func handPointerBehavior(HandPointerBehavior?) -> some View

Sets the behavior of the hand pointer while the user is interacting with the view.

struct HandPointerBehavior

A behavior that can be applied to the hand pointer while the user is interacting with a view.

