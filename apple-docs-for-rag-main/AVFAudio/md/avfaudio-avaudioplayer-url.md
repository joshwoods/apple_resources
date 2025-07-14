

- AVFAudio
- AVAudioPlayer
-  url 

Instance Property

# url

The URL of the audio file.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var url: URL? { get }
```

## Discussion

This property is nil if you don’t create the player with a URL.

## See Also

### Inspecting the audio data

var data: Data?

The audio data associated with the player.

var format: AVAudioFormat

The format of the player’s audio data.

var settings: [String : Any]

A dictionary that provides information about the player’s audio data.

