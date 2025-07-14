

- AVFAudio
- AVAudioSession
-  inputGain 

Instance Property

# inputGain

The gain applied to inputs associated with the session.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var inputGain: Float { get }
```

## Discussion

This property returns a floating point value ranging from `0.0` to `1.0`, where `0.0` represents the lowest gain setting, and `1.0` represents the highest gain setting.

You can observe changes to the value of this property by using key-value observing. For more information, see Using Key-Value Observing in Swift.

## See Also

### Setting input gain

var isInputGainSettable: Bool

A Boolean value that indicates whether you can set the input gain.

func setInputGain(Float) throws

Changes the input gain to the specified value.

