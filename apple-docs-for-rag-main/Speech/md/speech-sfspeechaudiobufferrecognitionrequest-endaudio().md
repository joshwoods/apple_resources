

- Speech
- SFSpeechAudioBufferRecognitionRequest
-  endAudio() 

Instance Method

# endAudio()

Marks the end of audio input for the recognition request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func endAudio()
```

## Discussion

Call this method explicitly to let the speech recognizer know that no more audio input is coming.

## See Also

### Appending Audio Buffers

func append(AVAudioPCMBuffer)

Appends audio in the PCM format to the end of the recognition request.

func appendAudioSampleBuffer(CMSampleBuffer)

Appends audio to the end of the recognition request.

