

- Network
- NWPathMonitor
-  init(prohibitedInterfaceTypes:) 

Initializer

# init(prohibitedInterfaceTypes:)

Initializes a path monitor to observe interface types that are not explicitly prohibited.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(prohibitedInterfaceTypes: [NWInterface.InterfaceType])
```

## See Also

### Creating Path Monitors

init()

Initializes a path monitor to observe all available interface types.

init(requiredInterfaceType: NWInterface.InterfaceType)

Initializes a path monitor to observe a specific interface type.

func start(queue: DispatchQueue)

Starts monitoring path changes, and sets a queue on which to deliver path events.

var queue: DispatchQueue?

The queue on which path events are delivered.

