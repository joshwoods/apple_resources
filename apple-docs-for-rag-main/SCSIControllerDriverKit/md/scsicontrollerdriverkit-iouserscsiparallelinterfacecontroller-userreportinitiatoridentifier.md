

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserReportInitiatorIdentifier 

Instance Method

# UserReportInitiatorIdentifier

Gets the SCSI device identifier for the host bus adapter (HBA) in response to a call from the framework.

DriverKit

``` source
kern_return_t UserReportInitiatorIdentifier(uint64_t * id);
```

## Parameters 

`id`  

On return, set this to the value of the initiator identifier.

## Return Value

A value that indicates the result of getting the initiator identifier. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

The framework calls this method to determine the SCSI device identifier that the initiator has assigned for this HBA.

## See Also

### Managing Host Bus Adapters

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

UserDoesHBASupportSCSIParallelFeature

Determines whether the driver extension class supports a specific feature in response to a call from the framework.

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

