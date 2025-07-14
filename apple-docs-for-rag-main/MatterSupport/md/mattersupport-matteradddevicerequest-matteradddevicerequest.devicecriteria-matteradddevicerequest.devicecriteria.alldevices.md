

- MatterSupport
- MatterAddDeviceRequest
- MatterAddDeviceRequest.DeviceCriteria
-  MatterAddDeviceRequest.DeviceCriteria.allDevices 

Case

# MatterAddDeviceRequest.DeviceCriteria.allDevices

All device match without any filtering.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
case allDevices
```

## See Also

### Defining the criteria

case all([MatterAddDeviceRequest.DeviceCriteria])

A device matches the given criteria if it matches all of the individual ones

case any([MatterAddDeviceRequest.DeviceCriteria])

A device matches the given criteria if it matches any one of the individual ones .

case commissioningID(UUID)

A device matches if it has the given commissioning identifier.

case fabricNode(rootPublicKey: Data, nodeID: UInt64)

A device matches if it’s paired to a fabric using the provided fabric and node identifiers.

case not(MatterAddDeviceRequest.DeviceCriteria)

A device matches the given criteria if it does not match the provided criteria.

case productID(Int)

A device matches if it has the given product identifier.

case serialNumber(String)

A device matches if it has the given product identifier.

case vendorID(Int)

A device matches if it has the given vendor.

