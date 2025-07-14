

- GameKit
- GKVoiceChatService
-  isOutputMeteringEnabled Deprecated

Instance Property

# isOutputMeteringEnabled

A Boolean value that indicates whether the voice level of remote participants is monitored.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var isOutputMeteringEnabled: Bool { get set }
```

Deprecated

Use SharePlay instead

## Discussion

If true, your application can read the outputMeterLevel property to monitor sound level of remote participants. If false, the value of the outputMeterLevel property is undefined. Default is false. When your application doesn’t need to monitor remote participants, it should set this property to false to improve performance.

## See Also

### Monitoring the Audio Level

var isInputMeteringEnabled: Bool

A Boolean value that indicates whether the microphone’s sound level is being monitored.

Deprecated

var inputMeterLevel: Float

The volume, in decibels (db), being received by the microphone.

Deprecated

var outputMeterLevel: Float

The volume, in decibels (db), being received from all other participants.

Deprecated

