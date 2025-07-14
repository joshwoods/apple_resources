

- GameKit
- GKVoiceChatService
-  isInputMeteringEnabled Deprecated

Instance Property

# isInputMeteringEnabled

A Boolean value that indicates whether the microphone’s sound level is being monitored.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var isInputMeteringEnabled: Bool { get set }
```

Deprecated

Use SharePlay instead

## Discussion

If true, your application can read the inputMeterLevel property to monitor the sound level of the microphone. If false, the value of the inputMeterLevel property is undefined. Default is false. When your application doesn’t need to monitor the microphone, it should set this property to false to improve performance.

## See Also

### Monitoring the Audio Level

var inputMeterLevel: Float

The volume, in decibels (db), being received by the microphone.

Deprecated

var isOutputMeteringEnabled: Bool

A Boolean value that indicates whether the voice level of remote participants is monitored.

Deprecated

var outputMeterLevel: Float

The volume, in decibels (db), being received from all other participants.

Deprecated

