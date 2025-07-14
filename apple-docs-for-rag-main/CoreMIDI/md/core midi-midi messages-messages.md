

- Core MIDI
-  MIDI Messages 

API Collection

# MIDI Messages

Create and configure messages.

## Topics

### MIDI 1.0 Messages

func MIDI1UPNoteOn(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPNoteOff(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPPitchBend(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPControlChange(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPSystemCommon(UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDI1UPChannelVoiceMessage(UInt8, UInt8, UInt8, UInt8, UInt8) -> MIDIMessage_32

func MIDIMessageTypeForUPWord(UInt32) -> MIDIMessageType

### MIDI 2.0 Messages

func MIDI2ChannelVoiceMessage(UInt8, UInt8, UInt8, UInt16, UInt32) -> MIDIMessage_64

func MIDI2NoteOn(UInt8, UInt8, UInt8, UInt8, UInt16, UInt16) -> MIDIMessage_64

func MIDI2NoteOff(UInt8, UInt8, UInt8, UInt8, UInt16, UInt16) -> MIDIMessage_64

func MIDI2ControlChange(UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2ProgramChange(UInt8, UInt8, Bool, UInt8, UInt8, UInt8) -> MIDIMessage_64

func MIDI2PitchBend(UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2PerNotePitchBend(UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2ChannelPressure(UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2PolyPressure(UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2AssignableControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RelRegisteredControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2AssignablePNC(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RegisteredPNC(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RelAssignableControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2RegisteredControl(UInt8, UInt8, UInt8, UInt8, UInt32) -> MIDIMessage_64

func MIDI2PerNoteManagment(UInt8, UInt8, UInt8, Bool, Bool) -> MIDIMessage_64

### Common

enum MIDICVStatus

MIDI status types.

enum MIDIProtocolID

Specifies a MIDI protocol variant.

enum MIDISysExStatus

MIDI System Exclusive (SysEx) types.

enum MIDISystemStatus

MIDI System status types.

struct MIDIMessage_128

A 128-bit MIDI message.

struct MIDIMessage_96

A 96-bit MIDI message.

struct MIDIMessage_64

A 64-bit MIDI message.

typealias MIDIMessage_32

A 32-bit MIDI message.

enum MIDIMessageType

Supported MIDI message types.

## See Also

### Services

MIDI Services

Communicate with hardware using Universal MIDI Packets.

MIDI System Setup

Configure the global MIDI system.

MIDI Bluetooth

Connect to Bluetooth Low Energy MIDI peripherals.

MIDI Thru Connection

Create play-through connections between sources and destinations.

MIDI Networking

Create and manage devices connected over a local network.

MIDI Drivers

Create driver plug-ins.

MIDI Capability Inquiry

Provide support for bidirectional discovery and configuration of devices.

