

- AVFAudio
- AVAudioConverter
-  convert(to:error:withInputFrom:) 

Instance Method

# convert(to:error:withInputFrom:)

Performs a conversion between audio formats, if the system supports it.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func convert(
    to outputBuffer: AVAudioBuffer,
    error outError: NSErrorPointer,
    withInputFrom inputBlock: @escaping AVAudioConverterInputBlock
) -> AVAudioConverterOutputStatus
```

## Parameters 

`outputBuffer`  

The output audio buffer.

`outError`  

The error if the conversion fails.

`inputBlock`  

A block the framework calls to get input data.

## Return Value

An AVAudioConverterOutputStatus type that indicates the conversion status.

## Discussion

The method attempts to fill the buffer to its capacity. On return, the buffer’s length indicates the number of sample frames the framework successfully converts.

## Topics

### Callbacks

typealias AVAudioConverterInputBlock

A block to get input data for conversion, as necessary.

## See Also

### Converting Audio Formats

func convert(to: AVAudioPCMBuffer, from: AVAudioPCMBuffer) throws

Performs a basic conversion between audio formats that doesn’t involve converting codecs or sample rates.

enum AVAudioConverterInputStatus

An option that indicates the status of an audio converter input block.

enum AVAudioConverterOutputStatus

An option that indicates the return status of an audio converter method.

