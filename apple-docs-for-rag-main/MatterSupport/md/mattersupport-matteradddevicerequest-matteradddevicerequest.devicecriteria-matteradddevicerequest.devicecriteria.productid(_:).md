

- MatterSupport
- MatterAddDeviceRequest
- MatterAddDeviceRequest.DeviceCriteria
-  MatterAddDeviceRequest.DeviceCriteria.productID(\_:) 

Case

# MatterAddDeviceRequest.DeviceCriteria.productID(\_:)

A device matches if it has the given product identifier.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
case productID(Int)
```

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

case fabricNode(rootPublicKey: Data, nodeID: UInt64)

A device matches if it’s paired to a fabric using the provided fabric and node identifiers.

case not(MatterAddDeviceRequest.DeviceCriteria)

A device matches the given criteria if it does not match the provided criteria.

case serialNumber(String)

A device matches if it has the given product identifier.

case vendorID(Int)

A device matches if it has the given vendor.

