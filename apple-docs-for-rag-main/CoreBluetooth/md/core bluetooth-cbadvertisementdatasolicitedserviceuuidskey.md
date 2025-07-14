

- Core Bluetooth
-  CBAdvertisementDataSolicitedServiceUUIDsKey 

Global Variable

# CBAdvertisementDataSolicitedServiceUUIDsKey

An array of solicited service UUIDs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBAdvertisementDataSolicitedServiceUUIDsKey: String
```

## Discussion

The value associated with this key is an array of one or more CBUUID objects, representing CBService UUIDs.

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

let CBAdvertisementDataTxPowerLevelKey: String

The transmit power of a peripheral.

let CBAdvertisementDataIsConnectable: String

A Boolean value that indicates whether the advertising event type is connectable.

