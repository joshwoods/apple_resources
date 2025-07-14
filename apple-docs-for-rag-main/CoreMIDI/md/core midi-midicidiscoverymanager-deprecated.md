

- Core MIDI
-  MIDICIDiscoveryManager Deprecated

Class

# MIDICIDiscoveryManager

A singleton object that performs systemwide MIDI-CI discovery.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class MIDICIDiscoveryManager
```

Deprecated

No longer supported for CoreMIDI

## Overview

Use this class to retrieve information about MIDI-CI–capable nodes in the MIDI subsystem. You can create MIDICISession objects only from the destinations discovered using this API.

## Topics

### Accessing the Shared Instance

class func sharedInstance() -> MIDICIDiscoveryManager

Returns the singleton discovery manager instance.

### Discovering Nodes

func discover(handler: MIDICIDiscoveryResponseBlock)

Discovers the available MIDI-CI nodes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Capability Inquiry

class MIDICISession

An object that represents a MIDI-CI session.

Deprecated

class MIDICIProfile

A mapping of MIDI messages to specific sounds and synthesis behaviors, such as General MIDI, a drawbar organ, and so on.

class MIDICIProfileState

An object that provides the enabled and disabled profiles for a MIDI channel or port on a device.

class MIDICIResponder

An object that responds to MIDI-CI inquiries from an initiator on behalf of a MIDI client, and handles profile and property exchange operations.

Deprecated

