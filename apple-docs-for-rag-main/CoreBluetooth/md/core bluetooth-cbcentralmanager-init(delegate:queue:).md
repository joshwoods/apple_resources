

- Core Bluetooth
- CBCentralManager
-  init(delegate:queue:) 

Initializer

# init(delegate:queue:)

Initializes the central manager with a specified delegate and dispatch queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    delegate: (any CBCentralManagerDelegate)?,
    queue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

The delegate that receives central events.

`queue`  

The dispatch queue used to dispatch the central role events. If the value is `nil`, the central manager dispatches central role events using the main queue.

## Return Value

Returns a newly initialized central manager.

## Discussion

For more information, see Core Bluetooth Programming Guide.

## See Also

### Initializing a Central Manager

convenience init()

Initializes the central manager without a delegate.

init(delegate: (any CBCentralManagerDelegate)?, queue: dispatch_queue_t?, options: [String : Any]?)

Initializes the central manager with specified delegate, dispatch queue, and initialization options.

Central Manager Initialization Options

Keys used to pass options when initializing a central manager.

Central Manager State Restoration Options

Keys used to pass state restoration options to the central manager initializer.

