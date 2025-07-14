

- Foundation
-  Streams, Sockets, and Ports 

API Collection

# Streams, Sockets, and Ports

Use low-level Unix features to manage input and output among files, processes, and the network.

## Topics

### Streams

class Stream

An abstract class representing a stream.

class InputStream

A stream that provides read-only stream functionality.

class OutputStream

A stream that provides write-only stream functionality.

protocol StreamDelegate

An interface that delegates of a stream instance use to handle events on the stream.

### Tasks and Pipes

class Process

An object that represents a subprocess of the current process.

class Pipe

A one-way communications channel between related processes.

### Sockets

class Host

A representation of an individual host on the network.

Deprecated

class Port

An abstract class that represents a communication channel.

class SocketPort

A port that represents a BSD socket.

### Byte Ordering

Byte Order Utilities

Examine and manage the byte order of numbers communicated through network channels.

## See Also

### Low-Level Utilities

XPC

Manage secure interprocess communication.

Object Runtime

Get low-level support for basic Objective-C features, Cocoa design patterns, and Swift integration.

Processes and Threads

Manage your app’s interaction with the host operating system and other processes, and implement low-level concurrency features.

