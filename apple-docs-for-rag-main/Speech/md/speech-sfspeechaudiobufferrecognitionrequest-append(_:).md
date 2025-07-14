

- Speech
- SFSpeechAudioBufferRecognitionRequest
-  append(\_:) 

Instance Method

# append(\_:)

Appends audio in the PCM format to the end of the recognition request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func append(_ audioPCMBuffer: AVAudioPCMBuffer)
```

## Parameters 

`audioPCMBuffer`  

An audio buffer that contains audio in the PCM format.

## Discussion

The audio must be in a native format and uncompressed.

## See Also

### Appending Audio Buffers

func appendAudioSampleBuffer(CMSampleBuffer)

Appends audio to the end of the recognition request.

func endAudio()

Marks the end of audio input for the recognition request.

