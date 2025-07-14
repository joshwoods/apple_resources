

- SpriteKit
- SKKeyframeSequence
-  sample(atTime:) 

Instance Method

# sample(atTime:)

Calculates the sample at a particular time.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func sample(atTime time: CGFloat) -> Any?
```

## Parameters 

`time`  

The time value to sample.

## Return Value

An object that contains the interpolated sample. The class of this object matches the class of the values stored in the keyframe sequence — either an NSNumber or an `SKColor`.

## Mentioned in 

Using Keyframe Sequence to effect Custom Interpolation

