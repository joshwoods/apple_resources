

- SceneKit
-  SCNAnimationEvent 

Class

# SCNAnimationEvent

A container for a closure, a block in Objective-C, to be executed at a specific time during playback of an animation.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNAnimationEvent
```

## Overview

Use animation events to add actions to animations, such as playing a sound to coincide with the movement of an animated character, or removing a node from the scene after playing an animation that fades out its visible geometry.

After you create an animation event, you attach it to an animation object using the object’s animationEvents property.

## Topics

### Creating an Animation Event

convenience init(keyTime: CGFloat, block: SCNAnimationEventBlock)

Creates an animation event.

### Constants

typealias SCNAnimationEventBlock

Signature for the block called when an animation event triggers.

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

### Explicit Animation

protocol SCNAnimatable

The common interface for attaching animations to nodes, geometries, materials, and other SceneKit objects.

class SCNAnimation

class SCNAnimationPlayer

class SCNTimingFunction

protocol SCNAnimationProtocol

class SCNAnimation

