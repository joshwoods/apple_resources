

- AVFAudio
- AVAudioFile
-  url 

Instance Property

# url

The location of the audio file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var url: URL { get }
```

## See Also

### Getting Audio File Properties

var fileFormat: AVAudioFormat

The on-disk format of the file.

var processingFormat: AVAudioFormat

The processing format of the file.

var length: AVAudioFramePosition

The number of sample frames in the file.

typealias AVAudioFramePosition

A position in an audio file or stream.

var framePosition: AVAudioFramePosition

The position in the file where the next read or write operation occurs.

typealias AVAudioFrameCount

A number of audio sample frames.

let AVAudioFileTypeKey: String

A string that indicates the audio file type.

var isOpen: Bool

A Boolean value that indicates whether the file is open.

