

- GameplayKit
-  GKPath 

Class

# GKPath

A polygonal path that can be followed by an agent.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKPath
```

## Overview

To make an agent move to or stay within the area defined by a path, create a goal with the init(toStayOn:maxPredictionTime:) method; to make an agent traverse along a path, create a goal with the init(toFollow:maxPredictionTime:forward:) method.

A path can be expressed as a sequence of either 2D points or 3D points. Use the former to create paths for use by GKAgent2D objects, and the latter to create paths for GKAgent3D objects to follow.

Note

The coordinate system in which you express the path’s vertices and radius is arbitrary; you may choose how to map agent positions and sizes into your game scene. It often makes sense to use the same coordinate system as your game engine—for example, when using agents in a SpriteKit-based game, you’d typically specify a path in screen points.

To learn more about using goals and agents, see Agents, Goals, and Behaviors in GameplayKit Programming Guide.

## Topics

### Creating a Path

init(graphNodes: [GKGraphNode], radius: Float)

Initializes a path using the positions of the specified graph nodes.

### Managing a Path’s Attributes

var radius: Float

The radius of the path.

var isCyclical: Bool

A Boolean value that determines whether the path loops around on itself (that is, the path’s end point connects to its start point).

### Inspecting a Path’s Shape

var numPoints: Int

The number of vertices in the path.

func float2(at: Int) -> vector_float2

Returns the 2D point at the specified index in the path’s list of vertices.

func float3(at: Int) -> vector_float3

Returns the 3D point at the specified index in the path’s list of vertices.

func point(at: Int) -> vector_float2

Returns the 2D point at the specified index in the path’s list of vertices.

Deprecated

### Initializers

convenience init(points: [SIMD3&lt;Float>], radius: Float, cyclical: Bool)

convenience init(points: [SIMD2&lt;Float>], radius: Float, cyclical: Bool)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Agents, Goals, and Behaviors

class GKAgent

A component that moves a game entity according to a set of goals and realistic constraints.

class GKAgent2D

An agent that operates in a two-dimensional space.

class GKAgent3D

An agent that operates in a three-dimensional space.

class GKGoal

An influence that motivates the movement of one or more agents.

class GKBehavior

A set of goals that together influence the movement of an agent.

class GKCompositeBehavior

A set of behaviors, each of which is a set of goals, that together influence the movement of an agent.

protocol GKAgentDelegate

Implement this protocol to synchronize the state of an agent with its visual representation in your game.

