

- Core Bluetooth
- CBPeripheralManager
-  Advertising Data 

API Collection

# Advertising Data

## Topics

### Advertising Keys

let CBAdvertisementDataIsConnectable: String

A Boolean value that indicates whether the advertising event type is connectable.

let CBAdvertisementDataLocalNameKey: String

The local name of a peripheral.

let CBAdvertisementDataManufacturerDataKey: String

The manufacturer data of a peripheral.

let CBAdvertisementDataOverflowServiceUUIDsKey: String

An array of UUIDs found in the overflow area of the advertisement data.

let CBAdvertisementDataServiceDataKey: String

A dictionary that contains service-specific advertisement data.

let CBAdvertisementDataServiceUUIDsKey: String

An array of service UUIDs.

let CBAdvertisementDataSolicitedServiceUUIDsKey: String

An array of solicited service UUIDs.

let CBAdvertisementDataTxPowerLevelKey: String

The transmit power of a peripheral.

## See Also

### Managing Advertising

func startAdvertising([String : Any]?)

Advertises peripheral manager data.

func stopAdvertising()

Stops advertising peripheral manager data.

var isAdvertising: Bool

A Boolean value that indicates whether the peripheral is advertising data.

