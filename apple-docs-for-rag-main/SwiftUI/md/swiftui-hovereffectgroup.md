

- SwiftUI
-  HoverEffectGroup 

Structure

# HoverEffectGroup

Describes a grouping of effects that activate together.

visionOS 2.0+

``` source
struct HoverEffectGroup
```

## Overview

Use HoverEffectGroup to apply effects to multiple views in concert.

## Topics

### Structures

struct Behavior

Describes the behavior of an effect in a group.

### Initializers

init(Namespace.ID, behavior: HoverEffectGroup.Behavior)

Creates a new HoverEffectGroup from a `Namespace.ID`.

init(id: String?, in: Namespace.ID, behavior: HoverEffectGroup.Behavior)

Creates a new HoverEffectGroup.

### Instance Methods

func behavior(HoverEffectGroup.Behavior) -> HoverEffectGroup

Returns a new version of `self` with the given `behavior`.

## Relationships

### Conforms To

- Equatable
- Sendable

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

