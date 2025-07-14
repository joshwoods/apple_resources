

- ShazamKit
- SHSignatureGenerator
-  signature() 

Instance Method

# signature()

Converts the audio buffer into a signature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func signature() -> SHSignature
```

## Return Value

A signature that ShazamKit generates from the audio buffer.

## See Also

### Generating a signature from audio

func append(AVAudioPCMBuffer, at: AVAudioTime?) throws

Adds audio to the generator.

Generating a signature from an audio buffer

Create a signature from an audio file or the microphone for a reference track in a custom catalog, or for matching tracks in a catalog.

