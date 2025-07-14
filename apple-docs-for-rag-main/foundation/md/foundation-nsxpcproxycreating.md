

- Foundation
-  NSXPCProxyCreating 

Protocol

# NSXPCProxyCreating

Methods for creating new proxy objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSXPCProxyCreating
```

## Overview

NSXPCConnection implements this protocol. All objects returned from the methods in this protocol also implement the protocol. This allows creation of new proxies from other proxies.

## Topics

### Instance Methods

func remoteObjectProxy() -> Any

Returns a proxy object with no error handling block.

**Required**

func remoteObjectProxyWithErrorHandler((any Error) -> Void) -> Any

Returns a proxy object that invokes the error handling block if an error occurs on the connection.

**Required**

func synchronousRemoteObjectProxyWithErrorHandler((any Error) -> Void) -> Any

## Relationships

### Conforming Types

- NSXPCConnection

## See Also

### XPC Client

class NSXPCConnection

A bidirectional communication channel between two processes.

class NSXPCInterface

An interface that may be sent to an exported object or remote object proxy.

class NSXPCCoder

A coder that encodes and decodes objects that your app sends over an XPC connection.

