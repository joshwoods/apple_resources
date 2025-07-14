

- Network
- NWProtocolFramerImplementation
-  label 

Type Property

# label

A label defined by your custom protocol for use in debugging.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var label: String { get }
```

**Required**

## See Also

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

