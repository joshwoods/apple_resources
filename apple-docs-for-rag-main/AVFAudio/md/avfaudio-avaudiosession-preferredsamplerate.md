

- AVFAudio
- AVAudioSession
-  preferredSampleRate 

Instance Property

# preferredSampleRate

The preferred sample rate, in hertz.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var preferredSampleRate: Double { get }
```

## Discussion

The value of this property indicates the preferred sample rate set using the setPreferredSampleRate(_:) method.

To determine the actual sample rate, query the sampleRate property.

## See Also

### Configuring sample rate

var sampleRate: Double

The current audio sample rate, in hertz.

func setPreferredSampleRate(Double) throws

Sets the preferred sample rate for audio input and output.

