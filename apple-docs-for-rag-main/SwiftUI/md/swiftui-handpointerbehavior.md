

- SwiftUI
-  HandPointerBehavior 

Structure

# HandPointerBehavior

A behavior that can be applied to the hand pointer while the user is interacting with a view.

visionOS 2.0+

``` source
struct HandPointerBehavior
```

## Topics

### Type Properties

static let drawing: HandPointerBehavior

Enables the hand pointer refined for drawing.

static let inactive: HandPointerBehavior

Deactivates the hand pointer inside the view. Use this to ensure the view will not apply any hand pointer behavior regardless of behaviors applied to ancestors in the hierarchy.

## Relationships

### Conforms To

- Equatable

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

protocol HoverEffectContent

A type that describes the effects of a view for a particular hover effect phase.

struct EmptyHoverEffectContent

An empty base effect that you use to build other effects.

func handPointerBehavior(HandPointerBehavior?) -> some View

Sets the behavior of the hand pointer while the user is interacting with the view.

