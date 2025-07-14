

- AVFAudio
- AVAudioEnvironmentOutputType
-  AVAudioEnvironmentOutputType.auto 

Case

# AVAudioEnvironmentOutputType.auto

Automatically detects the playback route and picks the correct output.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
case auto
```

## Discussion

When using the automatic output type, wired output defaults to AVAudioEnvironmentOutputType.headphones, and manual rendering with a two-channel output layout defaults to AVAudioEnvironmentOutputType.externalSpeakers.

## See Also

### Output Types

case headphones

Renders the audio output for headphones.

case builtInSpeakers

Renders the audio output for built-in speakers on the current hardware.

case externalSpeakers

Renders the audio output for external speakers according to the audio environment node’s output channel layout.

