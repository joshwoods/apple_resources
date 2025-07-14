

- Core Bluetooth
- CBPeripheralManager
-  delegate 

Instance Property

# delegate

The delegate object specified to receive peripheral events.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any CBPeripheralManagerDelegate)? { get set }
```

## Discussion

For information about how to implement your peripheral manager delegate, see CBPeripheralManagerDelegate.

## See Also

### Initializing a Peripheral Manager

convenience init()

Initializes the peripheral manager without a delegate.

convenience init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?)

Initializes the peripheral manager with a specified delegate and dispatch queue.

init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?, options: [String : Any]?)

Initializes the peripheral manager with a specified delegate, dispatch queue, and initialization options.

Peripheral Manager Initialization Options

Keys used to specify options when creating a peripheral manager.

