

- Speech
- SFSpeechAudioBufferRecognitionRequest
-  appendAudioSampleBuffer(\_:) 

Instance Method

# appendAudioSampleBuffer(\_:)

Appends audio to the end of the recognition request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func appendAudioSampleBuffer(_ sampleBuffer: CMSampleBuffer)
```

## Parameters 

`sampleBuffer`  

A buffer of audio.

## Discussion

The audio must be in a native format.

## See Also

### Appending Audio Buffers

func append(AVAudioPCMBuffer)

Appends audio in the PCM format to the end of the recognition request.

func endAudio()

Marks the end of audio input for the recognition request.

