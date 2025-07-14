

- Core MIDI
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Managing System Setup

typealias MIDISetupRef

A type that represents the global state of the MIDI system, that contains lists of the devices and serial port owners.

### Managing MIDI Devices

func MIDIDeviceAddEntity(MIDIDeviceRef, CFString, Bool, Int, Int, UnsafeMutablePointer&lt;MIDIEntityRef>) -> OSStatus

Specifies one of the entities that make up a device.

