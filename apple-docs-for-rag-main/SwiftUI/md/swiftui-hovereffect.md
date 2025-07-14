

- SwiftUI
-  HoverEffect 

Structure

# HoverEffect

An effect applied when the pointer hovers over a view.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 16.0+visionOS 1.0+

``` source
struct HoverEffect
```

## Topics

### Getting hover effects

static let automatic: HoverEffect

An effect that attempts to determine the effect automatically. This is the default effect.

static let highlight: HoverEffect

An effect that morphs the pointer into a platter behind the view and shows a light source indicating position.

static let lift: HoverEffect

An effect that slides the pointer under the view and disappears as the view scales up and gains a shadow.

### Initializers

init&lt;E>(E)

Create a `HoverEffect` that contains the specified custom hover effect.

## Relationships

### Conforms To

- Copyable
- CustomHoverEffect

## See Also

### Changing view appearance for hover events

func hoverEffect(HoverEffect) -> some View

Applies a hover effect to this view.

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

protocol HoverEffectContent

A type that describes the effects of a view for a particular hover effect phase.

struct EmptyHoverEffectContent

An empty base effect that you use to build other effects.

func handPointerBehavior(HandPointerBehavior?) -> some View

Sets the behavior of the hand pointer while the user is interacting with the view.

struct HandPointerBehavior

A behavior that can be applied to the hand pointer while the user is interacting with a view.

