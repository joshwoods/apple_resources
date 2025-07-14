

- SwiftUI
-  ScenePadding 

Structure

# ScenePadding

The padding used to space a view from its containing scene.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ScenePadding
```

## Overview

Add scene padding to a view using the scenePadding(_:edges:) modifier.

## Topics

### Getting padding values

static let minimum: ScenePadding

The minimum scene padding value.

static let navigationBar: ScenePadding

The navigation bar content scene padding.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Adding padding around a view

func padding(_:)

Adds a different padding amount to each edge of this view.

func padding(Edge.Set, CGFloat?) -> some View

Adds an equal padding amount to specific edges of this view.

func padding3D(_:)

Pads this view using the edge insets you specify.

func padding3D(Edge3D.Set, CGFloat?) -> some View

Pads this view using the edge insets you specify.

func scenePadding(Edge.Set) -> some View

Adds padding to the specified edges of this view using an amount that’s appropriate for the current scene.

func scenePadding(ScenePadding, edges: Edge.Set) -> some View

Adds a specified kind of padding to the specified edges of this view using an amount that’s appropriate for the current scene.

