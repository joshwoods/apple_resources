

- AVFAudio
- AVAudioFile
-  isOpen 

Instance Property

# isOpen

A Boolean value that indicates whether the file is open.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var isOpen: Bool { get }
```

## See Also

### Getting Audio File Properties

var url: URL

The location of the audio file.

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

