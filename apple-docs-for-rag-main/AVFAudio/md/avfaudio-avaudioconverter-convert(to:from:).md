

- AVFAudio
- AVAudioConverter
-  convert(to:from:) 

Instance Method

# convert(to:from:)

Performs a basic conversion between audio formats that doesn’t involve converting codecs or sample rates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func convert(
    to outputBuffer: AVAudioPCMBuffer,
    from inputBuffer: AVAudioPCMBuffer
) throws
```

## Parameters 

`outputBuffer`  

The output audio buffer.

`inputBuffer`  

The input audio buffer.

## Discussion

The output buffer’s frameCapacity value needs to be at least at large as the frameLength value of the `inputBuffer`.

## See Also

### Converting Audio Formats

func convert(to: AVAudioBuffer, error: NSErrorPointer, withInputFrom: AVAudioConverterInputBlock) -> AVAudioConverterOutputStatus

Performs a conversion between audio formats, if the system supports it.

enum AVAudioConverterInputStatus

An option that indicates the status of an audio converter input block.

enum AVAudioConverterOutputStatus

An option that indicates the return status of an audio converter method.

