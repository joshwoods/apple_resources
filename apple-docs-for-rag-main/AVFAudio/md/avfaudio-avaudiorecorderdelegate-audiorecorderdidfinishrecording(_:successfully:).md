

- AVFAudio
- AVAudioRecorderDelegate
-  audioRecorderDidFinishRecording(\_:successfully:) 

Instance Method

# audioRecorderDidFinishRecording(\_:successfully:)

Tells the delegate when recording stops or finishes due to reaching its time limit.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
optional func audioRecorderDidFinishRecording(
    _ recorder: AVAudioRecorder,
    successfully flag: Bool
)
```

## Parameters 

`recorder`  

The audio recorder that finished recording.

`flag`  

A Boolean value that indicates whether the recording stopped successfully.

## Discussion

The system doesn’t call this method if the recorder stops due to an interruption.

