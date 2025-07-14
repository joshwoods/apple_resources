

- Core Bluetooth
- CBCentralManagerDelegate
-  Advertisement Data Retrieval Keys 

API Collection

# Advertisement Data Retrieval Keys

Keys used to specify items in a dictionary of peripheral advertisement data.

## Topics

### Advertisement Keys

let CBAdvertisementDataLocalNameKey: String

The local name of a peripheral.

let CBAdvertisementDataManufacturerDataKey: String

The manufacturer data of a peripheral.

let CBAdvertisementDataServiceDataKey: String

A dictionary that contains service-specific advertisement data.

let CBAdvertisementDataServiceUUIDsKey: String

An array of service UUIDs.

let CBAdvertisementDataOverflowServiceUUIDsKey: String

An array of UUIDs found in the overflow area of the advertisement data.

let CBAdvertisementDataTxPowerLevelKey: String

The transmit power of a peripheral.

let CBAdvertisementDataIsConnectable: String

A Boolean value that indicates whether the advertising event type is connectable.

let CBAdvertisementDataSolicitedServiceUUIDsKey: String

An array of solicited service UUIDs.

## See Also

### Discovering and Retrieving Peripherals

func centralManager(CBCentralManager, didDiscover: CBPeripheral, advertisementData: [String : Any], rssi: NSNumber)

Tells the delegate the central manager discovered a peripheral while scanning for devices.

