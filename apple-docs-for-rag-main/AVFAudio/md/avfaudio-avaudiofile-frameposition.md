

- AVFAudio
- AVAudioFile
-  framePosition 

Instance Property

# framePosition

The position in the file where the next read or write operation occurs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var framePosition: AVAudioFramePosition { get set }
```

## Discussion

Set the `framePosition` property to perform a seek before a read or write. A read or write operation advances the frame position value by the number of frames it reads or writes.

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

typealias AVAudioFrameCount

A number of audio sample frames.

let AVAudioFileTypeKey: String

A string that indicates the audio file type.

var isOpen: Bool

A Boolean value that indicates whether the file is open.

