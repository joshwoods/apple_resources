

- AVFAudio
- AVAudioConverterOutputStatus
-  AVAudioConverterOutputStatus.inputRanDry 

Case

# AVAudioConverterOutputStatus.inputRanDry

A status that indicates the method doesn’t have enough input available to satisfy the request.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case inputRanDry
```

## Discussion

The output buffer contains as much data as the framework can convert.

## See Also

### Status Options

case haveData

A status that indicates that the method returns all of the requested data.

case endOfStream

A status that indicates the method reaches the end of the stream, and doesn’t return any data.

case error

A status that indicates the method encounters an error.

