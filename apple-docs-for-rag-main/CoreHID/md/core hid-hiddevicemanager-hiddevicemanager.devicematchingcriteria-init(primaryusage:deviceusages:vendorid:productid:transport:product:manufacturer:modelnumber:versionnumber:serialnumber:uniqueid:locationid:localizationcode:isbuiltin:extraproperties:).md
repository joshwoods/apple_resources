

- Core HID
- HIDDeviceManager
- HIDDeviceManager.DeviceMatchingCriteria
-  init(primaryUsage:deviceUsages:vendorID:productID:transport:product:manufacturer:modelNumber:versionNumber:serialNumber:uniqueID:locationID:localizationCode:isBuiltIn:extraProperties:) 

Initializer

# init(primaryUsage:deviceUsages:vendorID:productID:transport:product:manufacturer:modelNumber:versionNumber:serialNumber:uniqueID:locationID:localizationCode:isBuiltIn:extraProperties:)

Creates one set of matching criteria for HID devices.

macOS 15.0+

``` source
init(
    primaryUsage: HIDUsage? = nil,
    deviceUsages: [HIDUsage]? = nil,
    vendorID: UInt32? = nil,
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
    isBuiltIn: Bool? = nil,
    extraProperties: Dictionary? = nil
)
```

## Parameters 

`primaryUsage`  

See primaryUsage.

`deviceUsages`  

See deviceUsages.

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

`isBuiltIn`  

See isBuiltIn.

`extraProperties`  

A catch-all for uncommon or device specific criteria not listed above. This parameter is typically only for advanced users that need additional control over the matching process.

## Mentioned in 

Communicating with human interface devices

## Discussion

This `init` method is the only way to create matching criteria for discovering HID devices connected to the system. All parameters are optional; if none are specified, every discoverable device is matched.

Created HIDDeviceManager.DeviceMatchingCriteria are used by being passed to monitorNotifications(matchingCriteria:).

