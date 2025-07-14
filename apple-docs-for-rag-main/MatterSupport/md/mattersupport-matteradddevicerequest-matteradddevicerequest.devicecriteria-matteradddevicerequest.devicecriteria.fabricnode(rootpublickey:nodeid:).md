

- MatterSupport
- MatterAddDeviceRequest
- MatterAddDeviceRequest.DeviceCriteria
-  MatterAddDeviceRequest.DeviceCriteria.fabricNode(rootPublicKey:nodeID:) 

Case

# MatterAddDeviceRequest.DeviceCriteria.fabricNode(rootPublicKey:nodeID:)

A device matches if it’s paired to a fabric using the provided fabric and node identifiers.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
case fabricNode(
    rootPublicKey: Data,
    nodeID: UInt64
)
```

## Discussion

This will only match for devices already known to the system during the commissioning operation.

## See Also

### Defining the criteria

case allDevices

All device match without any filtering.

case all([MatterAddDeviceRequest.DeviceCriteria])

A device matches the given criteria if it matches all of the individual ones

case any([MatterAddDeviceRequest.DeviceCriteria])

A device matches the given criteria if it matches any one of the individual ones .

case commissioningID(UUID)

A device matches if it has the given commissioning identifier.

case not(MatterAddDeviceRequest.DeviceCriteria)

A device matches the given criteria if it does not match the provided criteria.

case productID(Int)

A device matches if it has the given product identifier.

case serialNumber(String)

A device matches if it has the given product identifier.

case vendorID(Int)

A device matches if it has the given vendor.

