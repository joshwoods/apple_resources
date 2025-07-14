

- AVFAudio
- AVAudioEnvironmentOutputType
-  AVAudioEnvironmentOutputType.builtInSpeakers 

Case

# AVAudioEnvironmentOutputType.builtInSpeakers

Renders the audio output for built-in speakers on the current hardware.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case builtInSpeakers
```

## Discussion

The output isn’t suitable for playback on other hardware.

In iOS devices, the rendering can be specific to device orientation. Manual rendering modes may not provide the rendering you expect if the device orientation changes between rendering the audio and playing it back.

## See Also

### Output Types

case auto

Automatically detects the playback route and picks the correct output.

case headphones

Renders the audio output for headphones.

case externalSpeakers

Renders the audio output for external speakers according to the audio environment node’s output channel layout.

