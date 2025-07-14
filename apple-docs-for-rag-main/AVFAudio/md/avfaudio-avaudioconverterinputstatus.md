

- AVFAudio
-  AVAudioConverterInputStatus 

Enumeration

# AVAudioConverterInputStatus

An option that indicates the status of an audio converter input block.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum AVAudioConverterInputStatus
```

## Topics

### Status Options

case endOfStream

A status that indicates you’re at the end of an audio stream.

case haveData

A status that indicates the normal case where you supply data to the converter.

case noDataNow

A status that indicates you’re out of data.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Converting Audio Formats

func convert(to: AVAudioBuffer, error: NSErrorPointer, withInputFrom: AVAudioConverterInputBlock) -> AVAudioConverterOutputStatus

Performs a conversion between audio formats, if the system supports it.

func convert(to: AVAudioPCMBuffer, from: AVAudioPCMBuffer) throws

Performs a basic conversion between audio formats that doesn’t involve converting codecs or sample rates.

enum AVAudioConverterOutputStatus

An option that indicates the return status of an audio converter method.

