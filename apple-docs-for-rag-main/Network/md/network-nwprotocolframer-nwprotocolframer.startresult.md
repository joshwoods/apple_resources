

- Network
- NWProtocolFramer
-  NWProtocolFramer.StartResult 

Enumeration

# NWProtocolFramer.StartResult

Results that you send to indicate the disposition of your protocol after receiving the call to start.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum StartResult
```

## Topics

### Start Results

case ready

The protocol is immediately ready to send and receive data.

case willMarkReady

The protocol will perform a handshake, preventing the overall connection from becoming ready until markReady() is called.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Handling Instance Lifetime

init(framer: NWProtocolFramer.Instance)

Initializes your custom framing protocol for use in one connection attempt.

**Required**

func start(framer: NWProtocolFramer.Instance) -> NWProtocolFramer.StartResult

Requests that your protocol set up its state and begin a handshake, if necessary.

**Required**

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

