

- Core Bluetooth
- CBPeripheralManager
-  Peripheral Manager Initialization Options 

API Collection

# Peripheral Manager Initialization Options

Keys used to specify options when creating a peripheral manager.

## Topics

### Initialization Options

let CBPeripheralManagerOptionShowPowerAlertKey: String

A Boolean value specifying whether the system should warn if Bluetooth is in the powered-off state when instantiating the peripheral manager.

let CBPeripheralManagerOptionRestoreIdentifierKey: String

A unique identifier (UID) with which to instantiate the peripheral manager.

## See Also

### Initializing a Peripheral Manager

convenience init()

Initializes the peripheral manager without a delegate.

convenience init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?)

Initializes the peripheral manager with a specified delegate and dispatch queue.

init(delegate: (any CBPeripheralManagerDelegate)?, queue: dispatch_queue_t?, options: [String : Any]?)

Initializes the peripheral manager with a specified delegate, dispatch queue, and initialization options.

var delegate: (any CBPeripheralManagerDelegate)?

The delegate object specified to receive peripheral events.

