

- Core Bluetooth
- CBCentralManager
-  Peripheral Scanning Options 

API Collection

# Peripheral Scanning Options

Keys used to pass options when scanning for peripherals.

## Topics

### Constants

let CBCentralManagerScanOptionAllowDuplicatesKey: String

A Boolean value that specifies whether the scan should run without duplicate filtering.

let CBCentralManagerScanOptionSolicitedServiceUUIDsKey: String

An array of service UUIDs that you want to scan for.

## See Also

### Scanning or Stopping Scans of Peripherals

func scanForPeripherals(withServices: [CBUUID]?, options: [String : Any]?)

Scans for peripherals that are advertising services.

func stopScan()

Asks the central manager to stop scanning for peripherals.

var isScanning: Bool

A Boolean value that indicates whether the central is currently scanning.

