

- Speech
- SFTranscriptionSegment
-  duration 

Instance Property

# duration

The number of seconds it took for the user to speak the utterance represented by the segment.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var duration: TimeInterval { get }
```

## Discussion

The duration contains the number of seconds it took for the user to speak the one or more words (utterance) represented by the segment. For example, the SFSpeechRecognizer sets duration to `0.6` if the user took `0.6` seconds to say `“time”` in the transcription of `“What time is it?"`.

## See Also

### Getting the Audio Timing Information

var timestamp: TimeInterval

The start time of the segment in the processed audio stream.

