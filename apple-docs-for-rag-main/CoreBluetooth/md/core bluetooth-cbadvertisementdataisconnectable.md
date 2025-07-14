

- Core Bluetooth
-  CBAdvertisementDataIsConnectable 

Global Variable

# CBAdvertisementDataIsConnectable

A Boolean value that indicates whether the advertising event type is connectable.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let CBAdvertisementDataIsConnectable: String
```

## Discussion

The value for this key is an NSNumber object. You can use this value to determine whether your app can currently connect to a peripheral.

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

let CBAdvertisementDataSolicitedServiceUUIDsKey: String

An array of solicited service UUIDs.

