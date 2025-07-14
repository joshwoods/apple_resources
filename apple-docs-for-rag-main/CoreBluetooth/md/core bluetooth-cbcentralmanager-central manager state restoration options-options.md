

- Core Bluetooth
- CBCentralManager
-  Central Manager State Restoration Options 

API Collection

# Central Manager State Restoration Options

Keys used to pass state restoration options to the central manager initializer.

## Topics

### State Restoration Options

let CBCentralManagerRestoredStatePeripheralsKey: String

An array of peripherals for use when restoring the state of a central manager.

let CBCentralManagerRestoredStateScanServicesKey: String

An array of service IDs for use when restoring state.

let CBCentralManagerRestoredStateScanOptionsKey: String

A dictionary of peripheral scan options for use when restoring state.

## See Also

### Initializing a Central Manager

convenience init()

Initializes the central manager without a delegate.

convenience init(delegate: (any CBCentralManagerDelegate)?, queue: dispatch_queue_t?)

Initializes the central manager with a specified delegate and dispatch queue.

init(delegate: (any CBCentralManagerDelegate)?, queue: dispatch_queue_t?, options: [String : Any]?)

Initializes the central manager with specified delegate, dispatch queue, and initialization options.

Central Manager Initialization Options

Keys used to pass options when initializing a central manager.

