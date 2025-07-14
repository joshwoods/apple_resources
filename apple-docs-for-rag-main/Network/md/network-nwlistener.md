

- Network
-  NWListener 

Class

# NWListener

An object you use to listen for incoming network connections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final class NWListener
```

## Mentioned in 

Creating an Identity for Local Network TLS

## Topics

### Creating Listeners

init(using: NWParameters, on: NWEndpoint.Port) throws

Initializes a network listener, with an optional local port.

func start(queue: DispatchQueue)

Registers for listening, and sets the queue on which all listener events are delivered.

var stateUpdateHandler: ((NWListener.State) -> Void)?

A handler that receives listener state updates.

enum State

States indicating whether a listener is able to accept incoming connections.

var port: NWEndpoint.Port?

The port on which the listener can accept connections.

func cancel()

Stops listening for inbound connections.

### Receiving Connections

var newConnectionHandler: ((NWConnection) -> Void)?

A handler that receives inbound connections.

var newConnectionLimit: Int

The remaining number of inbound connections to deliver before rejecting connections.

static let InfiniteConnectionLimit: Int

A static value to indicate that inbound connections should not be limited.

### Advertising Bonjour Services

NSBonjourServices

Bonjour service types browsed by the app.

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

var service: NWListener.Service?

A Bonjour service that advertises the listener on the local network.

struct Service

A description used to advertise the Bonjour service that a listener provides.

var serviceRegistrationUpdateHandler: ((NWListener.ServiceRegistrationChange) -> Void)?

A handler that receives updates for the service endpoint being advertised.

enum ServiceRegistrationChange

Changes to how a network listener’s service is advertised.

### Inspecting Listeners

let parameters: NWParameters

The parameters used to initialize the listener.

var queue: DispatchQueue?

The queue on which listener events are delivered.

### Initializers

convenience init(applicationService: String, using: NWParameters) throws

convenience init?(launchd: String, using: NWParameters)Deprecated

convenience init(launchdSocketKey: String, parameters: NWParameters)

convenience init(service: NWListener.Service, using: NWParameters) throws

### Instance Properties

var newConnectionGroupHandler: ((NWConnectionGroup) -> Void)?

var state: NWListener.State

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Connections and Listeners

class NWConnection

A bidirectional data connection between a local endpoint and a remote endpoint.

class NWBrowser

An object you use to browse for available network services.

class NWConnectionGroup

An object you use to communicate with a group of endpoints, such as an IP multicast group on a local network.

class NWEthernetChannel

An object you use to send and receive custom Ethernet frames.

