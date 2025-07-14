

- Core MIDI
-  MIDI2FlexDataMessage(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# MIDI2FlexDataMessage(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDI2FlexDataMessage(
    _ group: MIDIUInteger4,
    _ format: MIDIUInteger2,
    _ address: MIDIUInteger2,
    _ channel: MIDIUInteger4,
    _ statusBank: UInt8,
    _ status: UInt8,
    _ data1: UInt32,
    _ data2: UInt32,
    _ data3: UInt32
) -> MIDIMessage_128
```

## See Also

### Functions

func MIDI1UPChannelPressure(UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPPolyPressure(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPProgramChange(UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPSysEx(UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_64

func MIDI1UPSysExArray(UInt8, UInt8, UnsafePointer&lt;UInt8>!, UnsafePointer&lt;UInt8>!) -> MIDIMessage_64

func MIDI2EndOfClipMessage() -> MIDIMessage_128

func MIDI2EndpointDeviceIdentityNotificationMessage(MIDIUInteger7, MIDIUInteger7, MIDIUInteger7, MIDIUInteger14, MIDIUInteger14, MIDIUInteger28) -> MIDIMessage_128

func MIDI2EndpointDiscoveryMessage(UInt8, UInt8, Bool, Bool, Bool, Bool, Bool) -> MIDIMessage_128

func MIDI2EndpointInfoNotificationMessage(UInt8, UInt8, Bool, UInt8, Bool, Bool, Bool, Bool) -> MIDIMessage_128

func MIDI2EndpointNameNotificationMessage(UMPStreamMessageFormat, UnsafePointer&lt;CChar>!, Int) -> MIDIMessage_128

func MIDI2EndpointProductInstanceIDNotificationMessage(UMPStreamMessageFormat, UnsafePointer&lt;CChar>!, Int) -> MIDIMessage_128

func MIDI2FunctionBlockDiscoveryMessage(UInt8, Bool, Bool) -> MIDIMessage_128

func MIDI2FunctionBlockInfoNotificationMessage(Bool, MIDIUInteger7, MIDIUMPFunctionBlockUIHint, MIDIUMPFunctionBlockMIDI1Info, MIDIUMPFunctionBlockDirection, UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_128

func MIDI2FunctionBlockNameNotificationMessage(UMPStreamMessageFormat, UInt8, UnsafePointer&lt;CChar>!, Int) -> MIDIMessage_128

func MIDI2StartOfClipMessage() -> MIDIMessage_128

