

- Audio Toolbox
-  AUMIDIEventList 

Structure

# AUMIDIEventList

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AUMIDIEventList
```

## Topics

### Initializers

init()

init(next: UnsafeMutablePointer&lt;AURenderEvent>?, eventSampleTime: AUEventSampleTime, eventType: AURenderEventType, reserved: UInt8, cable: UInt8, eventList: MIDIEventList)

### Instance Properties

var cable: UInt8

var eventList: MIDIEventList

var eventSampleTime: AUEventSampleTime

var eventType: AURenderEventType

var next: UnsafeMutablePointer&lt;AURenderEvent>?

var reserved: UInt8

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct AudioConverterOptions

