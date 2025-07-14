

- AVFAudio
- AVAudioPlayer
-  delegate 

Instance Property

# delegate

The delegate object for the audio player.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
weak var delegate: (any AVAudioPlayerDelegate)? { get set }
```

## See Also

### Responding to player events

protocol AVAudioPlayerDelegate

A protocol that defines the methods to respond to audio playback events and decoding errors.

