

- SensorKit
- SRSpeechMetrics
-  sessionIdentifier 

Instance Property

# sessionIdentifier

An identifier for the audio session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var sessionIdentifier: String { get }
```

## Discussion

For example, this property is an identifier for a phone call or Siri utterance.

## See Also

### Getting session information

var sessionFlags: SRSpeechMetrics.SessionFlags

Details about the audio processing.

struct SessionFlags

Possible details about processing an audio stream.

var timeSinceAudioStart: TimeInterval

The number of seconds since the start of the audio stream.

var timestamp: Date

The date and time when the speech occurs.

