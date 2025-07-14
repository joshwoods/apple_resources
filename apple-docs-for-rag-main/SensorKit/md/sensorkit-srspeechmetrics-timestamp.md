

- SensorKit
- SRSpeechMetrics
-  timestamp 

Instance Property

# timestamp

The date and time when the speech occurs.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var timestamp: Date { get }
```

## See Also

### Getting session information

var sessionIdentifier: String

An identifier for the audio session.

var sessionFlags: SRSpeechMetrics.SessionFlags

Details about the audio processing.

struct SessionFlags

Possible details about processing an audio stream.

var timeSinceAudioStart: TimeInterval

The number of seconds since the start of the audio stream.

