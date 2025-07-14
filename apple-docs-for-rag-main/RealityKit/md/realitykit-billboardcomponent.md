

- RealityKit
-  BillboardComponent 

Structure

# BillboardComponent

A component that orients an entity instance so that it continuously points toward the active camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct BillboardComponent
```

## Overview

The `BillboardComponent` automatically adjusts an entity’s orientation so that its z-axis keeps pointing in the direction of the main camera in a RealityKit scene.

Add a `BillboardComponent` to any entity by passing it to an entity’s set(_:) method.

```
entity.components.set(BillboardComponent())
```

The entity immediately reorients itself so that it faces the scene’s active camera.

| Without `BillboardComponent` | With `BillboardComponent` |
|----|----|
|  |  |

Important

An entity with `BillboardComponent` doesn’t provide access to its end orientation. Requesting the entity’s orientation through its transform returns only the unaltered orientation.

For an example of how to animate blendFactor, see BillboardAction.

## Topics

### Initializers

init()

Creates a billboard component that points an entity’s positive z-axis directly toward the active camera.

### Instance Properties

var blendFactor: Float

The degree at which the entity rotates toward the camera.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Visual adjustments

struct HoverEffectComponent

A component that applies a visual effect to a hierarchy of entities when a person looks at or selects an entity.

