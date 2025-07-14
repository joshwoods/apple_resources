

- Network
-  NWProtocolFramerImplementation 

Protocol

# NWProtocolFramerImplementation

A protocol to which your classes can conform in order to implement a custom framing protocol.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol NWProtocolFramerImplementation : AnyObject
```

## Topics

### Handling Instance Lifetime

init(framer: NWProtocolFramer.Instance)

Initializes your custom framing protocol for use in one connection attempt.

**Required**

func start(framer: NWProtocolFramer.Instance) -> NWProtocolFramer.StartResult

Requests that your protocol set up its state and begin a handshake, if necessary.

**Required**

enum StartResult

Results that you send to indicate the disposition of your protocol after receiving the call to start.

func wakeup(framer: NWProtocolFramer.Instance)

Delivers a scheduled wakeup event.

**Required**

func stop(framer: NWProtocolFramer.Instance) -> Bool

Requests that your protocol send any final messages to close the connection.

**Required**

func cleanup(framer: NWProtocolFramer.Instance)

Indicates that your protocol should clean up all allocations before being deallocated.

**Required**

static var label: String

A label defined by your custom protocol for use in debugging.

**Required**

### Handling Data

func handleOutput(framer: NWProtocolFramer.Instance, message: NWProtocolFramer.Message, messageLength: Int, isComplete: Bool)

Notifies your protocol about a new outbound message.

**Required**

func handleInput(framer: NWProtocolFramer.Instance) -> Int

Notifies your protocol that new inbound data is available to parse.

**Required**

## See Also

### Implementing Framer Protocols

class Instance

An object that represents a single instance of your custom protocol running in a connection.

