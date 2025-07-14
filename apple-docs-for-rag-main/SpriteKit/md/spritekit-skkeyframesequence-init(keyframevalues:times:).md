

- SpriteKit
- SKKeyframeSequence
-  init(keyframeValues:times:) 

Initializer

# init(keyframeValues:times:)

Initializes a keyframe sequence with an initial set of values and times.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    keyframeValues values: [Any],
    times: [NSNumber]
)
```

## Parameters 

`values`  

An array of value objects that define the keyframe values for the sequence.

`times`  

An array of NSNumber objects containing floating-point values that specify the time values for the keyframes.

## Return Value

A newly initialized sequence.

## Discussion

The two arrays must have an identical number of elements. The keyframes in the new sequence are stored in the same order as the input arrays.

## See Also

### First Steps

Using Keyframe Sequence to effect Custom Interpolation

See a few examples of what keyframe sequence can do.

convenience init(capacity: Int)

Initializes a new keyframe sequence.

init?(coder: NSCoder)

