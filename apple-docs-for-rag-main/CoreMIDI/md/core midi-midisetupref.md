

- Core MIDI
-  MIDISetupRef 

Type Alias

# MIDISetupRef

A type that represents the global state of the MIDI system, that contains lists of the devices and serial port owners.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias MIDISetupRef = MIDIObjectRef
```

## Discussion

Derives from MIDIObjectRef, does not have an owner object.

Generally, only MIDI drivers and specialized configuration editors will need to manipulate MIDISetup objects, not the average MIDI client application. As of CoreMIDI 1.1, the MIDIServer maintains a single global MIDISetupRef, stored persistently in a preference file.

## See Also

### Data Types

typealias MIDICIDeviceID

struct DictionaryKey

typealias MIDICIMUID

struct MIDICIPropertyExchangeRequestID

typealias MIDIEventVisitor

typealias MIDIUInteger14

typealias MIDIUInteger2

typealias MIDIUInteger28

typealias MIDIUInteger4

typealias MIDIUInteger7

struct DictionaryKey

typealias MIDIUMPFunctionBlockID

typealias MIDIUMPGroupNumber

typealias MIDICIDiscoveryResponseBlock

A block the system calls when a MIDI-CI node discovery request completes.

Deprecated

typealias MIDICISessionDisconnectBlock

A block the system calls when a MIDI-CI session disconnects.

Deprecated

