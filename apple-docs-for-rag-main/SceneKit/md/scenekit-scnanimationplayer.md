

- SceneKit
-  SCNAnimationPlayer 

Class

# SCNAnimationPlayer

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class SCNAnimationPlayer
```

## Topics

### Initializers

init(animation: SCNAnimation)

### Instance Properties

var animation: SCNAnimation

var blendFactor: CGFloat

var paused: Bool

var speed: CGFloat

### Instance Methods

func play()

func stop()

func stop(withBlendOutDuration: TimeInterval)

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
- SCNAnimatable

## See Also

### Explicit Animation

protocol SCNAnimatable

The common interface for attaching animations to nodes, geometries, materials, and other SceneKit objects.

class SCNAnimationEvent

A container for a closure, a block in Objective-C, to be executed at a specific time during playback of an animation.

class SCNAnimation

class SCNTimingFunction

protocol SCNAnimationProtocol

class SCNAnimation

