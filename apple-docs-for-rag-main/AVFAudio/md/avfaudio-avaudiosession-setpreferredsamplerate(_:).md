

- AVFAudio
- AVAudioSession
-  setPreferredSampleRate(\_:) 

Instance Method

# setPreferredSampleRate(\_:)

Sets the preferred sample rate for audio input and output.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func setPreferredSampleRate(_ sampleRate: Double) throws
```

## Parameters 

`sampleRate`  

The hardware sample rate to use. The available range is device dependent and is typically from 8000 through 48000 hertz.

## Discussion

This method requests a change to the input and output audio sample rate. To see the effect of this change, use the sampleRate property.

You can set a preferred sample rate before or after activating the audio session.

## See Also

### Configuring sample rate

var sampleRate: Double

The current audio sample rate, in hertz.

var preferredSampleRate: Double

The preferred sample rate, in hertz.

