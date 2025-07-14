

- Network
- NWProtocolFramer
-  NWProtocolFramer.Instance 

Class

# NWProtocolFramer.Instance

An object that represents a single instance of your custom protocol running in a connection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final class Instance
```

## Overview

All interaction between your protocol and the connection occurs through this object.

## Topics

### Writing Output

func parseOutput(minimumIncompleteLength: Int, maximumLength: Int, parse: (UnsafeMutableRawBufferPointer?, Bool) -> Int) -> Bool

Examines the content of output data while inside your output handler.

func writeOutput(data: Data)

Sends arbitrary output data from your protocol to the next protocol.

func writeOutputNoCopy(length: Int) throws

Sends a specific number of bytes from a message while inside your output handler.

func passThroughOutput()

Indicates that your protocol no longer needs to handle output data.

### Delivering Input

func parseInput(minimumIncompleteLength: Int, maximumLength: Int, parse: (UnsafeMutableRawBufferPointer?, Bool) -> Int) -> Bool

Examines the content of input data while in your input handler.

func deliverInput(data: Data, message: NWProtocolFramer.Message, isComplete: Bool)

Delivers an inbound message containing arbitrary data from your protocol to the application.

func deliverInputNoCopy(length: Int, message: NWProtocolFramer.Message, isComplete: Bool) -> Bool

Delivers an inbound message containing a specific number of next received bytes.

func passThroughInput()

Indicates that your protocol no longer needs to handle input data.

### Managing Instance Lifetime

func markReady()

Indicates to a connection that your protocol’s handshake is complete.

func markFailed(error: NWError?)

Indicates to a connection that your protocol has encountered an error, or has gracefully closed.

func prependApplicationProtocol(options: NWProtocolOptions) throws

Dynamically adds another protocol that will run above your protocol after your protocol calls markReady().

### Inspecting Instance Properties

var remote: NWEndpoint?

The remote endpoint of the connection in which your protocol is running.

var local: NWEndpoint?

The local endpoint of the connection in which your protocol is running.

var parameters: NWParameters?

The parameters of the connection in which your protocol is running.

### Handling Asynchronous Events

func async(execute: () -> Void)

Requests that a block be executed on the connection’s internal scheduling context.

func scheduleWakeup(wakeupTime: NWProtocolFramer.Instance.WakeupTime)

Requests that wakeup(framer:) be called on your protocol at a specific time in the future.

enum WakeupTime

Times at which to schedule a protocol wakeup.

### Instance Properties

var options: NWProtocolFramer.Options

### Instance Methods

func writeOutput&lt;Output>(data: Output)

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Sendable

## See Also

### Implementing Framer Protocols

protocol NWProtocolFramerImplementation

A protocol to which your classes can conform in order to implement a custom framing protocol.

