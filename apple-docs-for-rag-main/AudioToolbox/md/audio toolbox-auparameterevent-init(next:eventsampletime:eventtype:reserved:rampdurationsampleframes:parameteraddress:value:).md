

- Audio Toolbox
- AUParameterEvent
-  init(next:eventSampleTime:eventType:reserved:rampDurationSampleFrames:parameterAddress:value:) 

Initializer

# init(next:eventSampleTime:eventType:reserved:rampDurationSampleFrames:parameterAddress:value:)

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    next: UnsafeMutablePointer?,
    eventSampleTime: AUEventSampleTime,
    eventType: AURenderEventType,
    reserved: (UInt8, UInt8, UInt8),
    rampDurationSampleFrames: AUAudioFrameCount,
    parameterAddress: AUParameterAddress,
    value: AUValue
)
```

