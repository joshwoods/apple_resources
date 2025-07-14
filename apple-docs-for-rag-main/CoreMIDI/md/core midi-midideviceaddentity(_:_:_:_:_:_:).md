

- Core MIDI
-  MIDIDeviceAddEntity(\_:\_:\_:\_:\_:\_:) 

Function

# MIDIDeviceAddEntity(\_:\_:\_:\_:\_:\_:)

Specifies one of the entities that make up a device.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.0–11.0DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func MIDIDeviceAddEntity(
    _ device: MIDIDeviceRef,
    _ name: CFString,
    _ embedded: Bool,
    _ numSourceEndpoints: Int,
    _ numDestinationEndpoints: Int,
    _ newEntity: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`device`  

The device to which an entity is to be added.

`name`  

The name of the new entity.

`embedded`  

True if this entity is inside the device, false if the entity simply consists of external connectors to which other devices can be attached.

`numSourceEndpoints`  

The number of source endpoints the entity has.

`numDestinationEndpoints`  

The number of destination endpoints the entity has.

`newEntity`  

On successful return, points to the newly-created entity.

## Return Value

An OSStatus result code.

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

func MIDI2FlexDataMessage(MIDIUInteger4, MIDIUInteger2, MIDIUInteger2, MIDIUInteger4, UInt8, UInt8, UInt32, UInt32, UInt32) -> MIDIMessage_128

func MIDI2FunctionBlockDiscoveryMessage(UInt8, Bool, Bool) -> MIDIMessage_128

func MIDI2FunctionBlockInfoNotificationMessage(Bool, MIDIUInteger7, MIDIUMPFunctionBlockUIHint, MIDIUMPFunctionBlockMIDI1Info, MIDIUMPFunctionBlockDirection, UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_128

func MIDI2FunctionBlockNameNotificationMessage(UMPStreamMessageFormat, UInt8, UnsafePointer&lt;CChar>!, Int) -> MIDIMessage_128

