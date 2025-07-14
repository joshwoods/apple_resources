

- SensorKit
- SRSpeechMetrics
-  sessionFlags 

Instance Property

# sessionFlags

Details about the audio processing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var sessionFlags: SRSpeechMetrics.SessionFlags { get }
```

## See Also

### Getting session information

var sessionIdentifier: String

An identifier for the audio session.

struct SessionFlags

Possible details about processing an audio stream.

var timeSinceAudioStart: TimeInterval

The number of seconds since the start of the audio stream.

var timestamp: Date

The date and time when the speech occurs.

