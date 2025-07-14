

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserReportHBAConstraints 

Instance Method

# UserReportHBAConstraints

Reports the I/O constraints for this controller.

DriverKit

``` source
kern_return_t UserReportHBAConstraints(OSDictionary * constraints);
```

## Parameters 

`constraints`  

A dictionary containing I/O constraint keys, and Boolean values indicating that the device supports the constraint. See the discussion for valid and required keys.

## Return Value

A value that indicates the result of reporting the HBA constraints. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

The valid keys for the `constraints` dictionary are as follows:

| Key name | Required? |
|----|----|
| kIOMaximumSegmentCountReadKey | Yes |
| kIOMaximumSegmentCountWriteKey | Yes |
| kIOMaximumSegmentByteCountReadKey | Yes |
| kIOMaximumSegmentByteCountWriteKey | Yes |
| kIOMinimumSegmentAlignmentByteCountKey | Yes |
| kIOMaximumSegmentAddressableBitCountKey | Yes |
| `kIOMinimumHBADataAlignmentMaskKey` | Yes |
| `kIOHierarchicalLogicalUnitSupportKey` | No |

Subclasses must call this method from the dext before UserInitializeController returns.

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

