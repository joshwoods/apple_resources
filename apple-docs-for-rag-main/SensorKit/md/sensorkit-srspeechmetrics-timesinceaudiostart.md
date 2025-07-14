

- SensorKit
- SRSpeechMetrics
-  timeSinceAudioStart 

Instance Property

# timeSinceAudioStart

The number of seconds since the start of the audio stream.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
var timeSinceAudioStart: TimeInterval { get }
```

## Discussion

When an audio stream starts, such as a phone call, SensorKit collects samples periodically. Use this field to determine the order of the samples in the audio stream.

## See Also

### Getting session information

var sessionIdentifier: String

An identifier for the audio session.

var sessionFlags: SRSpeechMetrics.SessionFlags

Details about the audio processing.

struct SessionFlags

Possible details about processing an audio stream.

var timestamp: Date

The date and time when the speech occurs.

