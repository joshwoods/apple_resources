

- GameKit
- GKVoiceChatService
-  inputMeterLevel Deprecated

Instance Property

# inputMeterLevel

The volume, in decibels (db), being received by the microphone.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var inputMeterLevel: Float { get }
```

Deprecated

Use SharePlay instead

## Discussion

The value of this property is undefined if isInputMeteringEnabled is set to false.

## See Also

### Monitoring the Audio Level

var isInputMeteringEnabled: Bool

A Boolean value that indicates whether the microphone’s sound level is being monitored.

Deprecated

var isOutputMeteringEnabled: Bool

A Boolean value that indicates whether the voice level of remote participants is monitored.

Deprecated

var outputMeterLevel: Float

The volume, in decibels (db), being received from all other participants.

Deprecated

