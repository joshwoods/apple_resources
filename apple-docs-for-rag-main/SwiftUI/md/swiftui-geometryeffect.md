

- SwiftUI
-  GeometryEffect 

Protocol

# GeometryEffect

An effect that changes the visual appearance of a view, largely without changing its ancestors or descendants.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol GeometryEffect : Animatable, ViewModifier, _RemoveGlobalActorIsolation where Self.Body == Never
```

## Overview

The only change the effect makes to the view’s ancestors and descendants is to change the coordinate transform to and from them.

## Topics

### Applying effects

func effectValue(size: CGSize) -> ProjectionTransform

Returns the current value of the effect.

**Required**

func ignoredByLayout() -> _IgnoredByLayoutEffect&lt;Self>

Returns an effect that produces the same geometry transform as this effect, but only applies the transform while rendering its view.

## Relationships

### Inherits From

- Animatable
- ViewModifier

## See Also

### Synchronizing geometries

func matchedGeometryEffect&lt;ID>(id: ID, in: Namespace.ID, properties: MatchedGeometryProperties, anchor: UnitPoint, isSource: Bool) -> some View

Defines a group of views with synchronized geometry using an identifier and namespace that you provide.

struct MatchedGeometryProperties

A set of view properties that may be synchronized between views using the `View.matchedGeometryEffect()` function.

struct Namespace

A dynamic property type that allows access to a namespace defined by the persistent identity of the object containing the property (e.g. a view).

func geometryGroup() -> some View

Isolates the geometry (e.g. position and size) of the view from its parent view.

