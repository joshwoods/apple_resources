

- Core MIDI
-  MIDIThruConnectionEndpoint 

Structure

# MIDIThruConnectionEndpoint

A source or destination in a MIDI thru connection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIThruConnectionEndpoint
```

## Overview

Set the endpoint’s uniqueID to 0 if the endpoint exists and you’re passing its endpointRef. When retrieving a connection from Core MIDI, its endpointRef may be `NULL` if it doesn’t exist, but the uniqueID is always non-zero.

## Topics

### Configuring an Endpoint

var uniqueID: MIDIUniqueID

The connection’s unique identifier.

var endpointRef: MIDIEndpointRef

The endpoint reference.

### Initializers

init()

init(endpointRef: MIDIEndpointRef, uniqueID: MIDIUniqueID)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Managing Connections

func MIDIThruConnectionCreate(CFString?, CFData, UnsafeMutablePointer&lt;MIDIThruConnectionRef>) -> OSStatus

Creates a MIDI thru connection.

func MIDIThruConnectionDispose(MIDIThruConnectionRef) -> OSStatus

Disposes a MIDI thru connection.

typealias MIDIThruConnectionRef

An opaque reference to a play-through connection.

Endpoint Configuration

Values that define the supported endpoint configurations.

