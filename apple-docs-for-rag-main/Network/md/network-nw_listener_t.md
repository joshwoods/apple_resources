

- Network
-  nw_listener_t 

Type Alias

# nw_listener_t

An object you use to listen for incoming network connections.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_listener_t = any OS_nw_listener
```

## Topics

### Creating Listeners

func nw_listener_create(nw_parameters_t) -> nw_listener_t?

Initializes a network listener, which will select a random port.

func nw_listener_create_with_port(UnsafePointer&lt;CChar>, nw_parameters_t) -> nw_listener_t?

Initializes a network listener with a specified local port.

func nw_listener_create_with_connection(nw_connection_t, nw_parameters_t) -> nw_listener_t?

Initializes a network listener to receive new streams on a multiplexed connection.

func nw_listener_set_queue(nw_listener_t, dispatch_queue_t)

Sets the queue on which all listener events are delivered.

func nw_listener_start(nw_listener_t)

Registers for listening for inbound connections.

func nw_listener_get_port(nw_listener_t) -> UInt16

The port on which the listener can accept connections.

func nw_listener_cancel(nw_listener_t)

Stops listening for inbound connections.

### Receiving Connections

func nw_listener_set_new_connection_handler(nw_listener_t, nw_listener_new_connection_handler_t?)

Sets a handler that receives inbound connections.

typealias nw_listener_new_connection_handler_t

A handler that delivers inbound connections.

func nw_listener_set_new_connection_limit(nw_listener_t, UInt32)

Resets the number of inbound connections to deliver before rejecting connections.

func nw_listener_get_new_connection_limit(nw_listener_t) -> UInt32

Checks the remaining number of inbound connections to deliver before rejecting connections.

var NW_LISTENER_INFINITE_CONNECTION_LIMIT: UInt32

A static value that indicates that inbound connections should not be limited.

### Advertising Bonjour Services

NSBonjourServices

Bonjour service types browsed by the app.

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

func nw_listener_set_advertise_descriptor(nw_listener_t, nw_advertise_descriptor_t?)

Sets a Bonjour service that advertises the listener on the local network.

typealias nw_advertise_descriptor_t

A description used to advertise the Bonjour service that a listener provides.

func nw_listener_set_advertised_endpoint_changed_handler(nw_listener_t, nw_listener_advertised_endpoint_changed_handler_t?)

Sets a handler that receives updates for the service endpoint being advertised.

typealias nw_listener_advertised_endpoint_changed_handler_t

A handler that indicates changes to the service endpoints being advertised as they are added and removed.

### Handling State Updates

func nw_listener_set_state_changed_handler(nw_listener_t, nw_listener_state_changed_handler_t?)

Sets a handler to receive listener state updates.

typealias nw_listener_state_changed_handler_t

A handler that delivers listener state updates with associated errors.

struct nw_listener_state_t

States indicating whether a listener is able to accept incoming connections.

