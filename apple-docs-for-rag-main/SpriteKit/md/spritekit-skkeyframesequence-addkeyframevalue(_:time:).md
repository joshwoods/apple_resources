

- SpriteKit
- SKKeyframeSequence
-  addKeyframeValue(\_:time:) 

Instance Method

# addKeyframeValue(\_:time:)

Adds a keyframe to the sequence.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func addKeyframeValue(
    _ value: Any,
    time: CGFloat
)
```

## Parameters 

`value`  

An object that defines the value to add. It must have the same class as other value objects stored in the sequence.

`time`  

The corresponding time.

## Discussion

The new keyframe is appended to the end of the array.

## See Also

### Sequence Building

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

