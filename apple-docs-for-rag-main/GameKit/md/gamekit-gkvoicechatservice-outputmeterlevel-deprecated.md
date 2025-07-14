

- GameKit
- GKVoiceChatService
-  outputMeterLevel Deprecated

Instance Property

# outputMeterLevel

The volume, in decibels (db), being received from all other participants.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var outputMeterLevel: Float { get }
```

Deprecated

Use SharePlay instead

## Discussion

The value of this property is undefined if isOutputMeteringEnabled is set to false.

The volume level is the aggregate volume of all remote participants, modified by the remoteParticipantVolume property.

## See Also

### Monitoring the Audio Level

var isInputMeteringEnabled: Bool

A Boolean value that indicates whether the microphone’s sound level is being monitored.

Deprecated

var inputMeterLevel: Float

The volume, in decibels (db), being received by the microphone.

Deprecated

var isOutputMeteringEnabled: Bool

A Boolean value that indicates whether the voice level of remote participants is monitored.

Deprecated

