

- AVFAudio
- AVAudioSession
-  mode 

Instance Property

# mode

The current audio session’s mode.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var mode: AVAudioSession.Mode { get }
```

## Discussion

The audio session mode, together with the audio session category, indicates to the system how you intend to use audio in your app. You can use a mode to configure the audio system for specific use cases such as video recording, voice or video chat, or audio analysis.

AVAudioSession.Mode discusses the values available for this property. The default value is default.

## See Also

### Inspecting mode configuration

var availableModes: [AVAudioSession.Mode]

The audio session modes available on the device.

struct Mode

Audio session mode identifiers.

