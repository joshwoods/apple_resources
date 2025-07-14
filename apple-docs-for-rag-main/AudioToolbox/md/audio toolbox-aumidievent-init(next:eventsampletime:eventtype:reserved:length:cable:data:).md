

- Audio Toolbox
- AUMIDIEvent
-  init(next:eventSampleTime:eventType:reserved:length:cable:data:) 

Initializer

# init(next:eventSampleTime:eventType:reserved:length:cable:data:)

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    next: UnsafeMutablePointer?,
    eventSampleTime: AUEventSampleTime,
    eventType: AURenderEventType,
    reserved: UInt8,
    length: UInt16,
    cable: UInt8,
    data: (UInt8, UInt8, UInt8)
)
```

