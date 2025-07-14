

- Foundation
-  NSXPCConnection 

Class

# NSXPCConnection

A bidirectional communication channel between two processes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSXPCConnection
```

## Overview

This class is the primary means of creating and configuring the communication mechanism between two processes. Each process has one instance of this class to represent the endpoint in the communication channel.

## Topics

### Creating a connection

init(listenerEndpoint: NSXPCListenerEndpoint)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in another process, identified by an NSXPCListenerEndpoint object.

init(machServiceName: String, options: NSXPCConnection.Options)

Initializes an NSXPCConnection object to connect to a LaunchAgent or LaunchDaemon with a name advertised in a `launchd.plist`.

struct Options

Options that you can pass to a connection.

init(serviceName: String)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in an XPC service, identified by a service name.

### Managing connection state

func activate()

Activates the connection.

func resume()

Starts or resumes handling of messages on a connection.

func invalidate()

Invalidates the connection.

func suspend()

Suspends the connection.

var interruptionHandler: (() -> Void)?

An interruption handler that is called if the remote process exits or crashes.

var invalidationHandler: (() -> Void)?

An invalidation handler that is called if the connection can not be formed or the connection has terminated and may not be re-established.

class func current() -> NSXPCConnection?

Returns the current connection, in the context of a call to a method on your exported object.

func scheduleSendBarrierBlock(() -> Void)

Add a barrier block to execute on the connection.

### Managing the connection interface

var serviceName: String?

The name of the XPC service that this connection was configured to connect to.

var endpoint: NSXPCListenerEndpoint

If the connection was created with an NSXPCListenerEndpoint object, returns the endpoint object used.

var exportedInterface: NSXPCInterface?

The NSXPCInterface object that describes the protocol for the exported object on this connection.

var exportedObject: Any?

An exported object for the connection.

var remoteObjectInterface: NSXPCInterface?

Defines the NSXPCInterface object that describes the protocol for the object represented by the `remoteObjectProxy`.

var remoteObjectProxy: Any

Returns a proxy for the remote object (that is, the `exportedObject` from the other side of this connection).

### Working with security attributes

var auditSessionIdentifier: au_asid_t

The BSM audit session identifier for the connecting process.

var processIdentifier: pid_t

The process ID (PID) of the connecting process.

var effectiveGroupIdentifier: gid_t

The effective group ID (EGID) of the connecting process.

var effectiveUserIdentifier: uid_t

The effective user ID (EUID) of the connecting process.

### Working with proxy objects

func remoteObjectProxyWithErrorHandler((any Error) -> Void) -> Any

Returns a proxy for the remote object (that is, the object exported from the other side of this connection) with the specified error handler.

func synchronousRemoteObjectProxyWithErrorHandler((any Error) -> Void) -> Any

### Working with code signing

func setCodeSigningRequirement(String)

Sets the code signing requirement for this connection.

### Error codes

var NSXPCConnectionInterrupted: Int

The XPC connection was interrupted.

var NSXPCConnectionInvalid: Int

The XPC connection was invalid.

var NSXPCConnectionReplyInvalid: Int

The XPC connection reply was invalid.

var NSXPCConnectionErrorMinimum: Int

The lower bounds of XPC connection error code values.

var NSXPCConnectionErrorMaximum: Int

The upper bounds of XPC connection error code values.

var NSXPCConnectionCodeSigningRequirementFailure: Int

A code-signing requirement check failed.

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
- NSXPCProxyCreating

## See Also

### XPC Client

protocol NSXPCProxyCreating

Methods for creating new proxy objects.

class NSXPCInterface

An interface that may be sent to an exported object or remote object proxy.

class NSXPCCoder

A coder that encodes and decodes objects that your app sends over an XPC connection.

