

- Network
-  NWConnectionGroup 

Class

# NWConnectionGroup

An object you use to communicate with a group of endpoints, such as an IP multicast group on a local network.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
final class NWConnectionGroup
```

## Topics

### Establishing Group Connectivity

init(with: any NWGroupDescriptor, using: NWParameters)

Initializes a new connection group with a group identifier.

class NWMulticastGroup

A descriptor for a group you use to join an IP multicast group on a local network.

protocol NWGroupDescriptor

A protocol that defines a group of endpoints with which you can communicate, such as a multicast group.

func start(queue: DispatchQueue)

Joins the group, registers to receive messages, and sets the queue on you handle group events.

### Sending and Receiving Group Messages

func setReceiveHandler(maximumMessageSize: Int, rejectOversizedMessages: Bool, handler: ((NWConnectionGroup.Message, Data?, Bool) -> Void)?)

Sets a handler that receives inbound messages from members of the group.

func send(content: Data?, to: NWEndpoint?, message: NWConnectionGroup.Message, completion: (NWError?) -> Void)

Sends data to the entire group, or to a specific member of the group.

class Message

An object that represents a message that you send or receive within a group, and that contains protocol metadata and send properties.

### Managing Groups

var stateUpdateHandler: ((NWConnectionGroup.State) -> Void)?

A handler that receives connection group state updates.

enum State

States that indicate whether you can use a connection group to send and receive messages.

var state: NWConnectionGroup.State

The current state of the connection group.

func cancel()

Cancels the connection group object and leaves the network group.

### Inspecting Groups

let descriptor: any NWGroupDescriptor

The descriptor of the group you use to initialize the connection group.

let parameters: NWParameters

The parameters with which you initialize the connection group.

var queue: DispatchQueue?

The queue on which you handle group events.

### Instance Properties

var newConnectionHandler: ((NWConnection) -> Void)?

### Instance Methods

func extract(connectionTo: NWEndpoint?, using: NWProtocolOptions?) -> NWConnection?

func metadata(definition: NWProtocolDefinition) -> NWProtocolMetadata?

func reinsert(connection: NWConnection) -> Bool

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

class NWEthernetChannel

An object you use to send and receive custom Ethernet frames.

