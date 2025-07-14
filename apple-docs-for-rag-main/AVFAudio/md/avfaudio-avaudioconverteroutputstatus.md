

- AVFAudio
-  AVAudioConverterOutputStatus 

Enumeration

# AVAudioConverterOutputStatus

An option that indicates the return status of an audio converter method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum AVAudioConverterOutputStatus
```

## Topics

### Status Options

case haveData

A status that indicates that the method returns all of the requested data.

case inputRanDry

A status that indicates the method doesn’t have enough input available to satisfy the request.

case endOfStream

A status that indicates the method reaches the end of the stream, and doesn’t return any data.

case error

A status that indicates the method encounters an error.

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

enum AVAudioConverterInputStatus

An option that indicates the status of an audio converter input block.

