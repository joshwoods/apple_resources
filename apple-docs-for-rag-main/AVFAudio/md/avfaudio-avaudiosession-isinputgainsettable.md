

- AVFAudio
- AVAudioSession
-  isInputGainSettable 

Instance Property

# isInputGainSettable

A Boolean value that indicates whether you can set the input gain.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var isInputGainSettable: Bool { get }
```

## Return Value

Returns true if the device allows input gain to be changed, otherwise false.

## Discussion

Not all devices support variable gain; check this property before attempting to set the input gain.

## See Also

### Setting input gain

var inputGain: Float

The gain applied to inputs associated with the session.

func setInputGain(Float) throws

Changes the input gain to the specified value.

