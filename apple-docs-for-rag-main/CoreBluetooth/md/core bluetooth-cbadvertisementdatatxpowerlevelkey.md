

- Core Bluetooth
-  CBAdvertisementDataTxPowerLevelKey 

Global Variable

# CBAdvertisementDataTxPowerLevelKey

The transmit power of a peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
let CBAdvertisementDataTxPowerLevelKey: String
```

## Discussion

The value associated with this key is an instance of NSNumber.

This key and value are available if the peripheral provides its transmitting power level in its advertising packet. You can calculate the path loss by comparing the RSSI value with the transmitting power level.

## See Also

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

let CBAdvertisementDataIsConnectable: String

A Boolean value that indicates whether the advertising event type is connectable.

let CBAdvertisementDataSolicitedServiceUUIDsKey: String

An array of solicited service UUIDs.

