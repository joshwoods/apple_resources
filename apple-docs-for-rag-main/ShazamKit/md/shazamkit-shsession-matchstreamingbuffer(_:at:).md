

- ShazamKit
- SHSession
-  matchStreamingBuffer(\_:at:) 

Instance Method

# matchStreamingBuffer(\_:at:)

Converts the audio in the buffer to a signature, and searches the reference signatures in the session catalog.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func matchStreamingBuffer(
    _ buffer: AVAudioPCMBuffer,
    at time: AVAudioTime?
)
```

## Parameters 

`buffer`  

An audio buffer.

`time`  

The start time of the audio to use for generating the signatures.

## Discussion

This method continues to generate signatures and perform searches until the audio in the buffer stops, which may result in multiple calls to the delegate.

The audio buffer must be in one of the supported formats. For the list of the supported audio formats, see append(_:at:).

To use the microphone as input for the buffer, see Matching audio using the built-in microphone.

Note

You must use the audio format of the first call to this method in the current session in all subsequent calls for the session.

## See Also

### Making a match

func match(SHSignature)

Searches for the query signature in the reference signatures that the session catalog contains.

Matching audio using the built-in microphone

Use the audio stream from the microphone as the source for a ShazamKit session.

