

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  ReportRemovability 

Instance Method

# ReportRemovability

Returns a Boolean value that indicates whether the media is removable, in response to a call from the framework.

DriverKit 21.0+

``` source
kern_return_t ReportRemovability(bool * isRemovable);
```

## Parameters 

`isRemovable`  

An in/out Boolean parameter. On output, set this to `true` if the hardware supports removable media.

## Return Value

A value that indicates the report-removability result. Return kIOReturnSuccess to inidicate success. To indicate a failure, see IOKit Constants for error definitions.

## See Also

### Reporting Device Capabilities

ReportEjectability

Returns a Boolean value that indicates whether the media is ejectable, in response to a call from the framework.

ReportWriteProtection

Returns a Boolean value that indicates whether the media is write protected, in response to a call from the framework.

