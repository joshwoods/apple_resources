

- Core Bluetooth
- CBPeripheralManagerDelegate
-  Peripheral Manager State Restoration Options 

API Collection

# Peripheral Manager State Restoration Options

Keys used to specify options when restoring the state of a peripheral manager.

## Topics

### State Restoration Dictionary Keys

let CBPeripheralManagerRestoredStateServicesKey: String

An array of restored peripheral services.

let CBPeripheralManagerRestoredStateAdvertisementDataKey: String

A dictionary of restored advertising data.

## See Also

### Monitoring Changes to the Peripheral Manager’s State

func peripheralManagerDidUpdateState(CBPeripheralManager)

Tells the delegate the peripheral manager’s state updated.

**Required**

func peripheralManager(CBPeripheralManager, willRestoreState: [String : Any])

Tells the delegate the system is about to restore the peripheral manager.

