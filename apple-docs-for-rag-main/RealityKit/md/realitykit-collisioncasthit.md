

- RealityKit
-  CollisionCastHit 

Structure

# CollisionCastHit

A hit result of a collision cast.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct CollisionCastHit
```

## Overview

You get a collection of collision cast hits from either the raycast(origin:direction:length:query:mask:relativeTo:) method, or the convexCast(convexShape:fromPosition:fromOrientation:toPosition:toOrientation:query:mask:relativeTo:) method. Each hit indicates where the ray or the convex shape, starting at a given point and traveling in a given direction, hit a particular entity in the scene.

The frame of reference for the position and normal of the hit depends on the reference entity parameter passed to the method that generated the hit. Pass `nil` as the reference to use world space.

## Topics

### Getting the entity

var entity: Entity

The entity that was hit.

### Characterizing the collision cast hit

var position: SIMD3&lt;Float>

The position of the hit.

var normal: SIMD3&lt;Float>

The normal of the hit.

var distance: Float

The distance from the ray origin to the hit, or the convex shape travel distance.

### Comparing collision cast hits

static func == (CollisionCastHit, CollisionCastHit) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Structures

struct TriangleHit

Information returned when ray intersects a triangle mesh.

### Instance Properties

var shapeIndex: Int

The index of the shape that was hit.

var triangleHit: CollisionCastHit.TriangleHit?

Information the system provides when a ray touches or intersects a triangle mesh.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Ray casting

struct TriangleHit

Information returned when ray intersects a triangle mesh.

enum CollisionCastQueryType

The kinds of ray and convex shape cast queries that you can make.

struct PixelCastHit

