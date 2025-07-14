

- SceneKit
-  SCNAnimation 

Class

# SCNAnimation

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class SCNAnimation
```

## Topics

### Supporting Types

typealias SCNAnimationDidStartBlock

typealias SCNAnimationDidStopBlock

### Initializers

init(caAnimation: CAAnimation)

init(contentsOf: URL)

init(named: String)

### Instance Properties

var animationDidStart: SCNAnimationDidStartBlock?

var animationDidStop: SCNAnimationDidStopBlock?

var animationEvents: [SCNAnimationEvent]?

var autoreverses: Bool

var blendInDuration: TimeInterval

var blendOutDuration: TimeInterval

var duration: TimeInterval

var fillsBackward: Bool

var fillsForward: Bool

var isAdditive: Bool

var isAppliedOnCompletion: Bool

var isCumulative: Bool

var isRemovedOnCompletion: Bool

var keyPath: String?

var repeatCount: CGFloat

var startDelay: TimeInterval

var timeOffset: TimeInterval

var timingFunction: SCNTimingFunction

var usesSceneTimeBase: Bool

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
- SCNAnimationProtocol

## See Also

### Explicit Animation

protocol SCNAnimatable

The common interface for attaching animations to nodes, geometries, materials, and other SceneKit objects.

class SCNAnimationEvent

A container for a closure, a block in Objective-C, to be executed at a specific time during playback of an animation.

class SCNAnimationPlayer

class SCNTimingFunction

protocol SCNAnimationProtocol

