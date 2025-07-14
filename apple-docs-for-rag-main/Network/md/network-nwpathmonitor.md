

- Network
-  NWPathMonitor 

Class

# NWPathMonitor

An observer that you use to monitor and react to network changes.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final class NWPathMonitor
```

## Topics

### Creating Path Monitors

init()

Initializes a path monitor to observe all available interface types.

init(requiredInterfaceType: NWInterface.InterfaceType)

Initializes a path monitor to observe a specific interface type.

init(prohibitedInterfaceTypes: [NWInterface.InterfaceType])

Initializes a path monitor to observe interface types that are not explicitly prohibited.

func start(queue: DispatchQueue)

Starts monitoring path changes, and sets a queue on which to deliver path events.

var queue: DispatchQueue?

The queue on which path events are delivered.

### Handling Path Updates

var currentPath: NWPath

The currently available network path observed by the path monitor.

var pathUpdateHandler: ((NWPath) -> Void)?

A handler that receives network path updates.

### Canceling Path Monitors

func cancel()

Stops receiving network path updates.

### Structures

struct Iterator

### Type Properties

static var ethernetChannel: NWPathMonitor

## Relationships

### Conforms To

- AsyncSequence
- Copyable
- CustomDebugStringConvertible
- Sendable

## See Also

### Paths and Interfaces

struct NWPath

An object that contains information about the properties of the network that a connection uses, or that are available to your app.

struct NWInterface

An interface that a network connection uses to send and receive data.

