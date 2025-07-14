

- MatterSupport
- MatterAddDeviceRequest
-  MatterAddDeviceRequest.DeviceCriteria 

Enumeration

# MatterAddDeviceRequest.DeviceCriteria

A predicate to match against possible devices that may appear in the picker.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
enum DeviceCriteria
```

## Topics

### Creating criteria

init(from: any Decoder) throws

Create the request from a decoder.

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

case productID(Int)

A device matches if it has the given product identifier.

case serialNumber(String)

A device matches if it has the given product identifier.

case vendorID(Int)

A device matches if it has the given vendor.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Defining the device criteria

var showDeviceCriteria: MatterAddDeviceRequest.DeviceCriteria

A predicate that filters what devices appear in the picker.

