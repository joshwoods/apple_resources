

- Core Bluetooth
-  CBAdvertisementDataServiceDataKey 

Global Variable

# CBAdvertisementDataServiceDataKey

A dictionary that contains service-specific advertisement data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
let CBAdvertisementDataServiceDataKey: String
```

## Discussion

The keys (CBUUID objects) represent CBService UUIDs, and the values (NSData objects) represent service-specific data.

## See Also

### Advertisement Keys

let CBAdvertisementDataLocalNameKey: String

The local name of a peripheral.

let CBAdvertisementDataManufacturerDataKey: String

The manufacturer data of a peripheral.

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

