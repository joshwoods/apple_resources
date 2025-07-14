

- Core MIDI
- MIDICIDiscoveryManager
-  discover(handler:) Deprecated

Instance Method

# discover(handler:)

Discovers the available MIDI-CI nodes.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func discover(handler completedHandler: @escaping MIDICIDiscoveryResponseBlock)
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`completedHandler`  

A closure the system calls when a MIDI-CI node discovery request is complete.

## Topics

### Handling Callbacks

typealias MIDICIDiscoveryResponseBlock

A block the system calls when a MIDI-CI node discovery request completes.

class MIDICIDiscoveredNode

A discovered MIDI-CI node that represents a MIDI source and destination that respond to capability inquiries.

