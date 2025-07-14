

- Core Bluetooth
- CBPeripheralManager
-  init(delegate:queue:) 

Initializer

# init(delegate:queue:)

Initializes the peripheral manager with a specified delegate and dispatch queue.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+

``` source
convenience init(
    delegate: (any CBPeripheralManagerDelegate)?,
    queue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

The delegate to receive the peripheral role events.

`queue`  

The dispatch queue for dispatching the peripheral role events. If the value is `nil`, the peripheral manager dispatches peripheral role events using the main queue.

## Return Value

Returns a newly initialized peripheral manager.

## Discussion

For more information, see Core Bluetooth Programming Guide.

## See Also

### Initializing a Peripheral Manager

convenience init()

Initializes the peripheral manager without a delegate.

init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?, options: [String : Any]?)

Initializes the peripheral manager with a specified delegate, dispatch queue, and initialization options.

var delegate: (any CBPeripheralManagerDelegate)?

The delegate object specified to receive peripheral events.

Peripheral Manager Initialization Options

Keys used to specify options when creating a peripheral manager.

