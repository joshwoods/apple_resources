

- ShazamKit
- SHSession
-  match(\_:) 

Instance Method

# match(\_:)

Searches for the query signature in the reference signatures that the session catalog contains.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func match(_ signature: SHSignature)
```

## Parameters 

`signature`  

The signature for searching the catalog of reference signatures.

## See Also

### Making a match

func matchStreamingBuffer(AVAudioPCMBuffer, at: AVAudioTime?)

Converts the audio in the buffer to a signature, and searches the reference signatures in the session catalog.

Matching audio using the built-in microphone

Use the audio stream from the microphone as the source for a ShazamKit session.

