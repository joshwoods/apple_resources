

- SpriteKit
- SKKeyframeSequence
-  setKeyframeValue(\_:for:) 

Instance Method

# setKeyframeValue(\_:for:)

Changes the value for a specific keyframe.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func setKeyframeValue(
    _ value: Any,
    for index: Int
)
```

## Parameters 

`value`  

The new value for the keyframe.

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

func setKeyframeValue(Any, time: CGFloat, for: Int)

Replaces a keyframe in the sequence with a new keyframe.

