

- Network
-  NWEthernetChannel 

Class

# NWEthernetChannel

An object you use to send and receive custom Ethernet frames.

macOS 10.15+

``` source
final class NWEthernetChannel
```

## Overview

Use Ethernet channels to send and receive custom Ethernet frame types over an interface.

Creating Ethernet channels requires the `com.apple.developer.networking.custom-protocol` entitlement.

## Topics

### Managing Ethernet Channels

init(on: NWInterface, etherType: UInt16)

Initializes an Ethernet channel on a specific interface with a custom Ethernet type.

func start(queue: DispatchQueue)

Starts the process of registering the channel, and sets the queue on which all channel events are delivered.

func cancel()

Unregisters the channel from the interface.

### Handling State Updates

var state: NWEthernetChannel.State

The current state of the channel.

enum State

States indicating whether an Ethernet channel is able to send and receive frames.

var stateUpdateHandler: ((NWEthernetChannel.State) -> Void)?

A handler that delivers channel state updates.

### Sending and Receiving Ethernet Frames

func send(content: Data, to: NWEthernetChannel.EthernetAddress, vlanTag: UInt16, completion: (NWError?) -> Void)

Sends a single Ethernet frame over a channel to a specific Ethernet address.

var receiveHandler: ((Data, UInt16, NWEthernetChannel.EthernetAddress, NWEthernetChannel.EthernetAddress) -> Void)?

A handler that delivers inbound Ethernet frames.

struct EthernetAddress

A 48-bit Ethernet address.

### Inspecting Ethernet Channels

let etherType: UInt16

The custom Ethernet type with which the channel was initialized.

let interface: NWInterface

The interface with which the channel was initialized.

var queue: DispatchQueue?

The queue on which channel events will be delivered.

### Initializers

init(on: NWInterface, etherType: UInt16, parameters: NWParameters)

### Instance Properties

var maximumPayloadSize: Int

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Connections and Listeners

class NWConnection

A bidirectional data connection between a local endpoint and a remote endpoint.

class NWListener

An object you use to listen for incoming network connections.

class NWBrowser

An object you use to browse for available network services.

class NWConnectionGroup

An object you use to communicate with a group of endpoints, such as an IP multicast group on a local network.

