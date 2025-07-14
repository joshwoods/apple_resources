

- AVFAudio
- AVAudioPlayer
-  data 

Instance Property

# data

The audio data associated with the player.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var data: Data? { get }
```

## Discussion

This property is nil if you don’t create the player with a data buffer.

## See Also

### Inspecting the audio data

var url: URL?

The URL of the audio file.

var format: AVAudioFormat

The format of the player’s audio data.

var settings: [String : Any]

A dictionary that provides information about the player’s audio data.

