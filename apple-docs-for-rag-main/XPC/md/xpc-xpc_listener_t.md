

- XPC
-  xpc_listener_t 

Type Alias

# xpc_listener_t

A C type that performs tasks for clients across process boundaries.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_listener_t = OS_xpc_listener
```

## Discussion

To implement an XPC service, create a listener and respond to incoming session requests.

## Topics

### Creating a listener

typealias xpc_listener_incoming_session_handler_t

A block that receives an incoming peer session request from a client.

### Working with code signing

func xpc_listener_set_peer_code_signing_requirement(xpc_listener_t, UnsafePointer&lt;CChar>) -> Int32

## See Also

### Interprocess communication

Creating XPC services

Configure a listener, establish a client session, and exchange messages between processes.

class XPCListener

A type that performs tasks for clients across process boundaries.

class XPCSession

A type that sends messages to a server process.

struct XPCReceivedMessage

A type that represents a message sent between a session and a listener.

typealias xpc_session_t

A C type that sends messages to a server process.

