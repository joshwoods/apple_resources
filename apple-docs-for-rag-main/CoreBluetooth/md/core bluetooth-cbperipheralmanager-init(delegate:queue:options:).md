

- Core Bluetooth
- CBPeripheralManager
-  init(delegate:queue:options:) 

Initializer

# init(delegate:queue:options:)

Initializes the peripheral manager with a specified delegate, dispatch queue, and initialization options.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+

``` source
init(
    delegate: (any CBPeripheralManagerDelegate)?,
    queue: dispatch_queue_t?,
    options: [String : Any]? = nil
)
```

## Parameters 

`delegate`  

The delegate to receive the peripheral role events.

`queue`  

The dispatch queue for dispatching the peripheral role events. If the value is `nil`, the peripheral manager dispatches peripheral role events using the main queue.

`options`  

An optional dictionary containing initialization options for a peripheral manager. For available options, see Peripheral Manager Initialization Options.

## Return Value

Returns a newly initialized peripheral manager.

## Discussion

This method is the designated initializer for the CBPeripheralManager class.

## See Also

### Initializing a Peripheral Manager

convenience init()

Initializes the peripheral manager without a delegate.

convenience init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?)

Initializes the peripheral manager with a specified delegate and dispatch queue.

var delegate: (any CBPeripheralManagerDelegate)?

The delegate object specified to receive peripheral events.

Peripheral Manager Initialization Options

Keys used to specify options when creating a peripheral manager.

