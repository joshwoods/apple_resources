

- Network Extension
-  NWTCPConnection Deprecated

Class

# NWTCPConnection

An object to manage a TCP connection, with or without TLS.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class NWTCPConnection
```

Deprecated

Use the nw_connection_t type from the Network framework instead.

## Topics

### Monitoring the connection status

var state: NWTCPConnectionState

The status of the connection.

enum NWTCPConnectionState

Defined connection states. New types may be defined in the future.

var isViable: Bool

The viability of a TCP connection indicates whether or not data can be transferred.

var error: (any Error)?

The connection-wide error property.

### Transferring data

func readMinimumLength(Int, maximumLength: Int, completionHandler: (Data?, (any Error)?) -> Void)

Read the requested range of bytes.

func readLength(Int, completionHandler: (Data?, (any Error)?) -> Void)

Read a certain number of bytes on a connection.

func write(Data, completionHandler: ((any Error)?) -> Void)

Write the data to the connection.

func writeClose()

Close the connection for writing.

### Canceling the connection

func cancel()

Cancel the connection.

### Responding to network changes

var hasBetterPath: Bool

If a connection has a better path, new connections would use a different interface.

init(upgradeFor: NWTCPConnection)

This convenience initializer can be used to create a new connection that will only be connected if there exists a better path (as determined by the system) to the remote endpoint of the original connection.

### Getting connection properties

var endpoint: NWEndpoint

The destination endpoint with which this connection was created.

var localAddress: NWEndpoint?

The IP address endpoint from which the connection was established.

var remoteAddress: NWEndpoint?

The IP address endpoint to which the connection was established.

var connectedPath: NWPath?

The network path over which the connection was established.

var txtRecord: Data?

The TXT record associated with a connected Bonjour service endpoint.

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

### TCP connections

class NWTLSParameters

TLS properties for creating a connection.

Deprecated

protocol NWTCPConnectionAuthenticationDelegate

A delegate protocol to customize the TLS authentication done by a connection.

Deprecated

