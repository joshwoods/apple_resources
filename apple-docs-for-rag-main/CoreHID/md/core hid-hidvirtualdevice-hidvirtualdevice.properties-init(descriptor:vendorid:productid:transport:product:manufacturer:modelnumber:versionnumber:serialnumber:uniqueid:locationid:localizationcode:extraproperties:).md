

- Core HID
- HIDVirtualDevice
- HIDVirtualDevice.Properties
-  init(descriptor:vendorID:productID:transport:product:manufacturer:modelNumber:versionNumber:serialNumber:uniqueID:locationID:localizationCode:extraProperties:) 

Initializer

# init(descriptor:vendorID:productID:transport:product:manufacturer:modelNumber:versionNumber:serialNumber:uniqueID:locationID:localizationCode:extraProperties:)

Creates a set of properties for a virtual device.

macOS 15.0+

``` source
init(
    descriptor: Data,
    vendorID: UInt32,
    productID: UInt32? = nil,
    transport: HIDDeviceTransport? = nil,
    product: String? = nil,
    manufacturer: String? = nil,
    modelNumber: String? = nil,
    versionNumber: UInt64? = nil,
    serialNumber: String? = nil,
    uniqueID: String? = nil,
    locationID: UInt64? = nil,
    localizationCode: HIDDeviceLocalizationCode? = nil,
    extraProperties: Dictionary? = nil
)
```

## Parameters 

`descriptor`  

See descriptor.

`vendorID`  

See vendorID.

`productID`  

See productID.

`transport`  

See transport.

`product`  

See product.

`manufacturer`  

See manufacturer.

`modelNumber`  

See modelNumber.

`versionNumber`  

See versionNumber.

`serialNumber`  

See serialNumber.

`uniqueID`  

See uniqueID.

`locationID`  

See locationID.

`localizationCode`  

See localizationCode.

`extraProperties`  

A catch-all for uncommon or device specific properties that aren’t listed above. This parameter is typically only for advanced users that need additional control over device functionality.

## Mentioned in 

Creating virtual devices

## Discussion

Properties must be specified during the creation of a virtual device using init(properties:).

