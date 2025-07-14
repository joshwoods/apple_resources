

- AVFAudio
- AVAudioRecorder
-  settings 

Instance Property

# settings

The settings that describe the format of the recorded audio.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
var settings: [String : Any] { get }
```

## Discussion

See init(url:settings:) for supported keys and values.

## See Also

### Inspecting the audio data

var url: URL

The URL to which the recorder writes its data.

var format: AVAudioFormat

The format of the recorded audio.

