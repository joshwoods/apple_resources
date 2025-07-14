

- SpriteKit
- SKKeyframeSequence
-  removeKeyframe(at:) 

Instance Method

# removeKeyframe(at:)

Removes a keyframe from the sequence.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func removeKeyframe(at index: Int)
```

## Parameters 

`index`  

The index of the keyframe value to remove.

## See Also

### Sequence Building

func addKeyframeValue(Any, time: CGFloat)

Adds a keyframe to the sequence.

func removeLastKeyframe()

Removes the last value in the sequence.

func setKeyframeTime(CGFloat, for: Int)

Changes the time for a specific keyframe.

func setKeyframeValue(Any, for: Int)

Changes the value for a specific keyframe.

func setKeyframeValue(Any, time: CGFloat, for: Int)

Replaces a keyframe in the sequence with a new keyframe.

