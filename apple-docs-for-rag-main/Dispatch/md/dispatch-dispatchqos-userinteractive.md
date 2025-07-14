

- Dispatch
- DispatchQoS
-  userInteractive 

Type Property

# userInteractive

The quality-of-service class for user-interactive tasks, such as animations, event handling, or updates to your app’s user interface.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
static let userInteractive: DispatchQoS
```

## Discussion

User-interactive tasks have the highest priority on the system. Use this class for tasks or queues that interact with the user or actively update your app’s user interface. For example, use this class for animations or for tracking events interactively.

## See Also

### Getting the Predefined QoS Objects

static let userInitiated: DispatchQoS

The quality-of-service class for tasks that prevent the user from actively using your app.

static let `default`: DispatchQoS

The default quality-of-service class.

static let utility: DispatchQoS

The quality-of-service class for tasks that the user does not track actively.

static let background: DispatchQoS

The quality-of-service class for maintenance or cleanup tasks that you create.

static let unspecified: DispatchQoS

The absence of a quality-of-service class.

