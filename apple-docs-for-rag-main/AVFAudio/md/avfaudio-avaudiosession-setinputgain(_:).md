

- AVFAudio
- AVAudioSession
-  setInputGain(\_:) 

Instance Method

# setInputGain(\_:)

Changes the input gain to the specified value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setInputGain(_ gain: Float) throws
```

## Parameters 

`gain`  

The new gain value, which must be in the range `0.0` to `1.0`, where `0.0` represents the lowest gain setting and `1.0` represents the highest gain setting.

## Discussion

Before calling this method, check the value in the isInputGainSettable property to make sure the input gain level is settable for the current inputs.

## See Also

### Setting input gain

var inputGain: Float

The gain applied to inputs associated with the session.

var isInputGainSettable: Bool

A Boolean value that indicates whether you can set the input gain.

