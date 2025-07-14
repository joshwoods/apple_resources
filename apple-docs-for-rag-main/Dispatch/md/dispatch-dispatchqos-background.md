

- Dispatch
- DispatchQoS
-  background 

Type Property

# background

The quality-of-service class for maintenance or cleanup tasks that you create.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
static let background: DispatchQoS
```

## Discussion

Background tasks have the lowest priority of all tasks. Assign this class to tasks or dispatch queues that you use to perform work while your app is running in the background.

## See Also

### Getting the Predefined QoS Objects

static let userInteractive: DispatchQoS

The quality-of-service class for user-interactive tasks, such as animations, event handling, or updates to your app’s user interface.

static let userInitiated: DispatchQoS

The quality-of-service class for tasks that prevent the user from actively using your app.

static let `default`: DispatchQoS

The default quality-of-service class.

static let utility: DispatchQoS

The quality-of-service class for tasks that the user does not track actively.

static let unspecified: DispatchQoS

The absence of a quality-of-service class.

