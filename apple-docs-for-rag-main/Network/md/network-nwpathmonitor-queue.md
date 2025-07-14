

- Network
- NWPathMonitor
-  queue 

Instance Property

# queue

The queue on which path events are delivered.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
final var queue: DispatchQueue? { get }
```

## See Also

### Creating Path Monitors

init()

Initializes a path monitor to observe all available interface types.

init(requiredInterfaceType: NWInterface.InterfaceType)

Initializes a path monitor to observe a specific interface type.

init(prohibitedInterfaceTypes: [NWInterface.InterfaceType])

Initializes a path monitor to observe interface types that are not explicitly prohibited.

func start(queue: DispatchQueue)

Starts monitoring path changes, and sets a queue on which to deliver path events.

