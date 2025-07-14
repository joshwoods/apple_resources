

- SceneKit
-  SCNAnimatable 

Protocol

# SCNAnimatable

The common interface for attaching animations to nodes, geometries, materials, and other SceneKit objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNAnimatable : NSObjectProtocol
```

## Mentioned in 

Animating SceneKit Content

## Overview

SceneKit uses the same architecture as the Core Animation framework, allowing you to animate property changes implicitly or explicitly. For implicit animation, use the SCNTransaction class to quickly create simple animations with very little code. For more complex animations, explicitly create CAAnimation objects, and use the methods in the SCNAnimatable protocol to attach them to the SceneKit objects you want to animate. You also use the methods in this protocol to control any animations already attached to a SceneKit object.

For example, making a node spin continuously for as long as it appears in the scene graph requires explicitly creating an animation that repeats. The following code creates such an animation and attaches it to a node:

```
CABasicAnimation *rotationAnimation = [CABasicAnimation animationWithKeyPath:@"rotation"];
// Animate one complete revolution around the node's Y axis.
rotationAnimation.toValue = [NSValue valueWithSCNVector4:SCNVector4Make(0, 1, 0, M_PI * 2)];
rotationAnimation.duration = 10.0; // One revolution in ten seconds.
rotationAnimation.repeatCount = FLT_MAX; // Repeat the animation forever.
[node addAnimation:rotationAnimation forKey:nil]; // Attach the animation to the node to start it.
```

## Topics

### Managing Animations

func addAnimation(any SCNAnimationProtocol, forKey: String?)

Adds an animation object for the specified key.

**Required**

func animation(forKey: String) -> CAAnimation?

Returns the animation with the specified key.

**Required**

Deprecated

var animationKeys: [String]

An array containing the keys of all animations currently attached to the object.

**Required**

func removeAllAnimations()

Removes all the animations currently attached to the object.

**Required**

func removeAnimation(forKey: String)

Removes the animation attached to the object with the specified key.

**Required**

func removeAnimation(forKey: String, fadeOutDuration: CGFloat)

Removes the animation attached to the object with the specified key, smoothly transitioning out of the animation’s effect.

**Required**

Deprecated

### Pausing and Resuming Animations

func pauseAnimation(forKey: String)

Pauses the animation attached to the object with the specified key.

**Required**

Deprecated

func resumeAnimation(forKey: String)

Resumes a previously paused animation attached to the object with the specified key.

**Required**

Deprecated

func isAnimationPaused(forKey: String) -> Bool

Returns a Boolean value indicating whether the animation attached to the object with the specified key is paused.

**Required**

Deprecated

### Instance Methods

func addAnimationPlayer(SCNAnimationPlayer, forKey: String?)

**Required**

func animationPlayer(forKey: String) -> SCNAnimationPlayer?

**Required**

func removeAllAnimations(withBlendOutDuration: CGFloat)

**Required**

func removeAnimation(forKey: String, blendOutDuration: CGFloat)

**Required**

func setAnimationSpeed(CGFloat, forKey: String)

**Required**

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SCNAccelerationConstraint
- SCNAnimationPlayer
- SCNAvoidOccluderConstraint
- SCNBillboardConstraint
- SCNBox
- SCNCamera
- SCNCapsule
- SCNCone
- SCNConstraint
- SCNCylinder
- SCNDistanceConstraint
- SCNFloor
- SCNGeometry
- SCNIKConstraint
- SCNLight
- SCNLookAtConstraint
- SCNMaterial
- SCNMaterialProperty
- SCNMorpher
- SCNNode
- SCNParticleSystem
- SCNPlane
- SCNPyramid
- SCNReferenceNode
- SCNReplicatorConstraint
- SCNShape
- SCNSliderConstraint
- SCNSphere
- SCNTechnique
- SCNText
- SCNTorus
- SCNTransformConstraint
- SCNTube

## See Also

### Explicit Animation

class SCNAnimationEvent

A container for a closure, a block in Objective-C, to be executed at a specific time during playback of an animation.

class SCNAnimation

class SCNAnimationPlayer

class SCNTimingFunction

protocol SCNAnimationProtocol

class SCNAnimation

