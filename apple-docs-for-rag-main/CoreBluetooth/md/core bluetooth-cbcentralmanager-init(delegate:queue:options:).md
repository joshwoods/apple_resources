

- Core Bluetooth
- CBCentralManager
-  init(delegate:queue:options:) 

Initializer

# init(delegate:queue:options:)

Initializes the central manager with specified delegate, dispatch queue, and initialization options.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    delegate: (any CBCentralManagerDelegate)?,
    queue: dispatch_queue_t?,
    options: [String : Any]? = nil
)
```

## Parameters 

`delegate`  

The delegate that receives the central events.

`queue`  

The dispatch queue used to dispatch the central role events. If the value is `nil`, the central manager dispatches central role events using the main queue.

`options`  

An optional dictionary that contains initialization options for a central manager. For available options, see Central Manager Initialization Options.

## Return Value

Returns a newly initialized central manager.

## Discussion

This method is the designated initializer for the CBCentralManager class.

## See Also

### Initializing a Central Manager

convenience init()

Initializes the central manager without a delegate.

convenience init(delegate: (any CBCentralManagerDelegate)?, queue: dispatch_queue_t?)

Initializes the central manager with a specified delegate and dispatch queue.

Central Manager Initialization Options

Keys used to pass options when initializing a central manager.

Central Manager State Restoration Options

Keys used to pass state restoration options to the central manager initializer.

