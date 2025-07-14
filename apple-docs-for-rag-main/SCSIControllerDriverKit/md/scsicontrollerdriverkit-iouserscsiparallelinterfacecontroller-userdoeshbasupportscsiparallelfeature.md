

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserDoesHBASupportSCSIParallelFeature 

Instance Method

# UserDoesHBASupportSCSIParallelFeature

Determines whether the driver extension class supports a specific feature in response to a call from the framework.

DriverKit

``` source
kern_return_t UserDoesHBASupportSCSIParallelFeature(uint32_t theValue, bool * result);
```

## Parameters 

`theValue`  

The SCSI parallel interconnect (SPI) feature to check.

`result`  

A pointer to a Boolean value. On return, set this value to `true` if it supports the feature, and `false` if it doesn’t.

## Return Value

A value that indicates the result of determining if the driver extension class supports the feature. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

The SCSI parallel interconnect standard defines the features that `theValue` specifies.

## See Also

### Managing Host Bus Adapters

UserReportInitiatorIdentifier

Gets the SCSI device identifier for the host bus adapter (HBA) in response to a call from the framework.

UserReportHighestSupportedDeviceID

Gets the highest supported SCSI device identifier in response to a call from the framework.

UserReportMaximumTaskCount

Gets the maximum number of outstanding tasks the HBA can process in response to a call from the framework.

UserDoesHBAPerformDeviceManagement

Determines if the host bus adapter (HBA) manages devices in response to a call from the framework.

UserReportHBAHighestLogicalUnitNumber

Gets the highest logical unit number (LUN) in response to a call from the framework.

UserDoesHBAPerformAutoSense

Determines if the driver extension class automatically performs autosense and provides autosense data for each I/O in response to a call from the framework.

UserDoesHBASupportMultiPathing

Queries the HBA child class to determine if it supports multipathing in response to a call from the framework.

SCSIParallelFeature

A feature that the driver extension supports.

UserMapHBAData

Maps any host bus adapter (HBA)-specific task data in response to a call from the framework.

UserSetHBAProperties

Sets multiple properties for a host bus adapter.

UserRemoveHBAProperties

Removes properties from a host bus adapter in response to a call from the framework.

UserReportHBAConstraints

Reports the I/O constraints for this controller.

