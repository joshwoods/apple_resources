

- SpriteKit
- SKKeyframeSequence
-  setKeyframeValue(\_:time:for:) 

Instance Method

# setKeyframeValue(\_:time:for:)

Replaces a keyframe in the sequence with a new keyframe.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setKeyframeValue(
    _ value: Any,
    time: CGFloat,
    for index: Int
)
```

## Parameters 

`value`  

The new value for the keyframe.

`time`  

The new time for the keyframe.

`index`  

The index of the keyframe to change.

## See Also

### Sequence Building

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

