

- SpriteKit
-  SKAction 

Class

# SKAction

An object that is run by a node to change its structure or content.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKAction
```

## Mentioned in 

Getting Started with Actions

Getting Started with Spring Joints

Working with Inverse Kinematics

## Overview

SKAction is an animation that is executed by a node in the scene. Actions are used to change a node in some way (like move its position over time), but you can also use actions to change the scene, like doing a fadeout. When the scene processes its nodes, the actions associated with those nodes are processed.

## Topics

### First Steps

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

Action Initializers

Use these functions to create actions.

### Controlling Action Timing

Configuring Action Timing

Time an action in a scene, by adding or modifying timing properties, or cancel an action.

var duration: TimeInterval

The duration required to complete an action.

var timingMode: SKActionTimingMode

A setting that controls the speed curve of an animation.

enum SKActionTimingMode

The modes that an action can use to adjust the apparent timing of the action.

var timingFunction: SKActionTimingFunction

A block used to customize the timing function.

typealias SKActionTimingFunction

The signature for the custom timing block.

var speed: CGFloat

A speed factor that modifies how fast an action runs.

### Using Action Names

Controlling Actions Precisely by Using Names

Set an action’s name property so you can access it later without needing an instance variable.

### Observing Live Changes

Detecting Changes at Each Step of an Animation

Get notified of a property change on your node subclass and retrieve the amount of change.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Animation

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

