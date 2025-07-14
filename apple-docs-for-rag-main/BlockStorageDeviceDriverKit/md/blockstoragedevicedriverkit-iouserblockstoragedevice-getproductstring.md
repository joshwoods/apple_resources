

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  GetProductString 

Instance Method

# GetProductString

Gets a string that identifies the product in response to a call from the framework.

DriverKit 21.0+

``` source
kern_return_t GetProductString(struct DeviceString * product);
```

## Parameters 

`product`  

An in/out DeviceString parameter. On output, populate this structure with the product string.

## Return Value

A value that indicates the get-product-string result. Return kIOReturnSuccess to inidicate success. To indicate a failure, see IOKit Constants for error definitions.

## See Also

### Reporting Device Metadata

GetVendorString

Gets a string that identifies the vendor in response to a call from the framework.

GetRevisionString

Gets a string that identifies the current revision in response to a call from the framework.

GetAdditionalInfoString

Gets a string that provides additional information in response to a call from the framework.

DeviceString

A type that represents a string of character data from the device.

GetDeviceParams

Gets device parameters in response to a call from the framework.

DeviceParams

A structure that represents hardware-specific properties of the block storage device.

