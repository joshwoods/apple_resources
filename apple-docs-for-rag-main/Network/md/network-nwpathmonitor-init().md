

- Network
- NWPathMonitor
-  init() 

Initializer

# init()

Initializes a path monitor to observe all available interface types.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init()
```

## See Also

### Creating Path Monitors

init(requiredInterfaceType: NWInterface.InterfaceType)

Initializes a path monitor to observe a specific interface type.

init(prohibitedInterfaceTypes: [NWInterface.InterfaceType])

Initializes a path monitor to observe interface types that are not explicitly prohibited.

func start(queue: DispatchQueue)

Starts monitoring path changes, and sets a queue on which to deliver path events.

var queue: DispatchQueue?

The queue on which path events are delivered.

