

- Core Bluetooth
- CBCentralManager
-  Central Manager Initialization Options 

API Collection

# Central Manager Initialization Options

Keys used to pass options when initializing a central manager.

## Topics

### Constants

let CBCentralManagerOptionShowPowerAlertKey: String

A Boolean value that specifies whether the system warns the user if the app instantiates the central manager when Bluetooth service isn’t available.

let CBCentralManagerOptionRestoreIdentifierKey: String

A string containing a unique identifier (UID) for the central manager to instantiate.

## See Also

### Initializing a Central Manager

convenience init()

Initializes the central manager without a delegate.

convenience init(delegate: (any CBCentralManagerDelegate)?, queue: dispatch_queue_t?)

Initializes the central manager with a specified delegate and dispatch queue.

init(delegate: (any CBCentralManagerDelegate)?, queue: dispatch_queue_t?, options: [String : Any]?)

Initializes the central manager with specified delegate, dispatch queue, and initialization options.

Central Manager State Restoration Options

Keys used to pass state restoration options to the central manager initializer.

