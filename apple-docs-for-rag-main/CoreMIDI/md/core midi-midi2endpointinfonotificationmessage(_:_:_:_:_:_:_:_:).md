

- Core MIDI
-  MIDI2EndpointInfoNotificationMessage(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# MIDI2EndpointInfoNotificationMessage(\_:\_:\_:\_:\_:\_:\_:\_:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func MIDI2EndpointInfoNotificationMessage(
    _ versionMajor: UInt8,
    _ versionMinor: UInt8,
    _ staticFunctionBlocks: Bool,
    _ numberOfFunctionBlocks: UInt8,
    _ m1: Bool,
    _ m2: Bool,
    _ receiveJRTimestamp: Bool,
    _ transmitJRTimestamp: Bool
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

func MIDI2EndpointNameNotificationMessage(UMPStreamMessageFormat, UnsafePointer&lt;CChar>!, Int) -> MIDIMessage_128

func MIDI2EndpointProductInstanceIDNotificationMessage(UMPStreamMessageFormat, UnsafePointer&lt;CChar>!, Int) -> MIDIMessage_128

func MIDI2FlexDataMessage(MIDIUInteger4, MIDIUInteger2, MIDIUInteger2, MIDIUInteger4, UInt8, UInt8, UInt32, UInt32, UInt32) -> MIDIMessage_128

func MIDI2FunctionBlockDiscoveryMessage(UInt8, Bool, Bool) -> MIDIMessage_128

func MIDI2FunctionBlockInfoNotificationMessage(Bool, MIDIUInteger7, MIDIUMPFunctionBlockUIHint, MIDIUMPFunctionBlockMIDI1Info, MIDIUMPFunctionBlockDirection, UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_128

func MIDI2FunctionBlockNameNotificationMessage(UMPStreamMessageFormat, UInt8, UnsafePointer&lt;CChar>!, Int) -> MIDIMessage_128

func MIDI2StartOfClipMessage() -> MIDIMessage_128

