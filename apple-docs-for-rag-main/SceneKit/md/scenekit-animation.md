

- SceneKit
-  Animation 

API Collection

# Animation

Create declarative animations that move elements of a scene in predetermined ways, or manage animations imported with external authoring tools.

## Topics

### First Steps

Animating SceneKit Content

Learn about implicit animations, explicit animations, and actions, and when to choose each in your app.

### Actions

class SCNAction

A simple, reusable animation that changes attributes of any node you attach it to.

protocol SCNActionable

Methods for running actions on nodes.

### Implicit Animation

class SCNTransaction

A mechanism for creating implicit animations and combining scene graph changes into atomic updates.

### Explicit Animation

protocol SCNAnimatable

The common interface for attaching animations to nodes, geometries, materials, and other SceneKit objects.

class SCNAnimationEvent

A container for a closure, a block in Objective-C, to be executed at a specific time during playback of an animation.

class SCNAnimation

class SCNAnimationPlayer

class SCNTimingFunction

protocol SCNAnimationProtocol

class SCNAnimation

## See Also

### Animation and Constraints

Constraints

Automatically adjust the position or orientation of a node based on specified rules.

class SCNSkinner

An object that manages the relationship between skeletal animations and the nodes and geometries they animate.

class SCNMorpher

An object that manages smooth transitions between a node’s base geometry and one or more target geometries.

