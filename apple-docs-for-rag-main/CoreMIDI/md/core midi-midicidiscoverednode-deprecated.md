

- Core MIDI
-  MIDICIDiscoveredNode Deprecated

Class

# MIDICIDiscoveredNode

A discovered MIDI-CI node that represents a MIDI source and destination that respond to capability inquiries.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class MIDICIDiscoveredNode
```

Deprecated

No longer supported for CoreMIDI

## Topics

### Inspecting a Node

var destination: MIDIEntityRef

The node’s MIDI destination.

var deviceInfo: MIDICIDeviceInfo

The available MIDI-CI device information.

var supportsProfiles: Bool

A Boolean value that indicates whether this node supports MIDI-CI profiles.

var supportsProperties: Bool

A Boolean value that indicates whether this node supports MIDI-CI properties.

var maximumSysExSize: NSNumber

The maximum size of a System Exclusive (SysEx) message this node supports.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Handling Callbacks

typealias MIDICIDiscoveryResponseBlock

A block the system calls when a MIDI-CI node discovery request completes.

Deprecated

