

- SpriteKit
-  SKKeyframeSequence 

Class

# SKKeyframeSequence

An object that performs interpolation between values specified at different times (keyframes).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKKeyframeSequence
```

## Mentioned in 

Using Keyframe Sequence to effect Custom Interpolation

Animating Particle Properties Across Disparate Values

## Overview

The primary use for an SKKeyframeSequence object is to animate properties on particles emitted by an SKEmitterNode object, but it can also be used for your general interpolation needs across a discrete set of inputs.

When a keyframe sequence is used with an emitter node, particles determine their values by sampling the keyframe sequence. The sequence replaces the normal simulation performed by the emitter node.

## Topics

### First Steps

Using Keyframe Sequence to effect Custom Interpolation

See a few examples of what keyframe sequence can do.

init(keyframeValues: [Any], times: [NSNumber])

Initializes a keyframe sequence with an initial set of values and times.

convenience init(capacity: Int)

Initializes a new keyframe sequence.

init?(coder: NSCoder)

### Sequence Building

Define the composition of the keyframe sequence.

func addKeyframeValue(Any, time: CGFloat)

Adds a keyframe to the sequence.

func removeKeyframe(at: Int)

Removes a keyframe from the sequence.

func removeLastKeyframe()

Removes the last value in the sequence.

func setKeyframeTime(CGFloat, for: Int)

Changes the time for a specific keyframe.

func setKeyframeValue(Any, for: Int)

Changes the value for a specific keyframe.

func setKeyframeValue(Any, time: CGFloat, for: Int)

Replaces a keyframe in the sequence with a new keyframe.

### Sequence Running

You run the sequence by sampling its output at a given time.

func sample(atTime: CGFloat) -> Any?

Calculates the sample at a particular time.

### Sequence Information

func count() -> Int

The number of keyframes in the sequence.

func getKeyframeTime(for: Int) -> CGFloat

Gets the time for a keyframe in the sequence.

func getKeyframeValue(for: Int) -> Any

Gets the value for a keyframe in the sequence.

### Interpolation Modifiers

Modify sample output by defining a mode or repeat options.

var interpolationMode: SKInterpolationMode

The mode used to determine how values for times between the keyframes are calculated.

var repeatMode: SKRepeatMode

The mode used to determine how the keyframe sequence repeats.

### Constants

enum SKInterpolationMode

The modes used to interpolate between keyframes in the sequence.

enum SKRepeatMode

The modes used to determine how the sequence repeats.

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

### Mathematical Tools

class SKRange

A definition of a range of floating-point values.

class SKRegion

The definition of an arbitrary area.

