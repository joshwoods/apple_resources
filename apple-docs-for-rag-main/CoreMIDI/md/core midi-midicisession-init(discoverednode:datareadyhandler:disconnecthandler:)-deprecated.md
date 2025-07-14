

- Core MIDI
- MIDICISession
-  init(discoveredNode:dataReadyHandler:disconnectHandler:) Deprecated

Initializer

# init(discoveredNode:dataReadyHandler:disconnectHandler:)

Creates a MIDI-CI session.

iOS 12.0–18.0DeprecatediPadOS 12.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
init(
    discoveredNode: MIDICIDiscoveredNode,
    dataReadyHandler handler: @escaping () -> Void,
    disconnectHandler: @escaping MIDICISessionDisconnectBlock
)
```

Deprecated

No longer supported for CoreMIDI

## Parameters 

`discoveredNode`  

A node found during discovery.

`handler`  

A block the system calls when the session’s data is ready.

`disconnectHandler`  

A block the system calls when you disconnect from the session.

## Topics

### Handling Callbacks

typealias MIDICISessionDisconnectBlock

A block the system calls when a MIDI-CI session disconnects.

