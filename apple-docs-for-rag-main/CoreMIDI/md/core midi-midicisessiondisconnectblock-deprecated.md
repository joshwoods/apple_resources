

- Core MIDI
-  MIDICISessionDisconnectBlock Deprecated

Type Alias

# MIDICISessionDisconnectBlock

A block the system calls when a MIDI-CI session disconnects.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
typealias MIDICISessionDisconnectBlock = (MIDICISession, any Error) -> Void
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`session`  

The disconnected session instance.

`error`  

An object that provides error information, if any.

## Discussion

If the system calls this block, terminate the MIDI-CI session.

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

typealias MIDIChannelNumber

