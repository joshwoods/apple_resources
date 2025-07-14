

- Speech
- SFTranscriptionSegment
-  timestamp 

Instance Property

# timestamp

The start time of the segment in the processed audio stream.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var timestamp: TimeInterval { get }
```

## Discussion

The timestamp is the number of seconds between the beginning of the audio content and when the user spoke the word represented by the segment. For example, if the user said the word “time” one second into the transcription “What time is it”, the timestamp would be equal to `1.0`.

## See Also

### Getting the Audio Timing Information

var duration: TimeInterval

The number of seconds it took for the user to speak the utterance represented by the segment.

