

- Foundation
-  XPC 

API Collection

# XPC

Manage secure interprocess communication.

## Topics

### XPC Client

protocol NSXPCProxyCreating

Methods for creating new proxy objects.

class NSXPCConnection

A bidirectional communication channel between two processes.

class NSXPCInterface

An interface that may be sent to an exported object or remote object proxy.

class NSXPCCoder

A coder that encodes and decodes objects that your app sends over an XPC connection.

### XPC Services

class NSXPCListener

A listener that waits for new incoming connections, configures them, and accepts or rejects them.

protocol NSXPCListenerDelegate

The protocol that delegates to the XPC listener use to accept or reject new connections.

class NSXPCListenerEndpoint

An object that names a specific XPC listener.

## See Also

### Low-Level Utilities

Object Runtime

Get low-level support for basic Objective-C features, Cocoa design patterns, and Swift integration.

Processes and Threads

Manage your app’s interaction with the host operating system and other processes, and implement low-level concurrency features.

Streams, Sockets, and Ports

Use low-level Unix features to manage input and output among files, processes, and the network.

