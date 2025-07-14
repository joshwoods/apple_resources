

- SCSIControllerDriverKit
- IOUserSCSIParallelInterfaceController
-  UserSetHBAProperties 

Instance Method

# UserSetHBAProperties

Sets multiple properties for a host bus adapter.

DriverKit

``` source
kern_return_t UserSetHBAProperties(OSDictionary * properties);
```

## Parameters 

`properties`  

A dictionary containing key-value pairs of properties.

## Return Value

A value that indicates the result of setting the properties. kIOReturnSuccess indicates success. For error definitions, see IOKit Constants.

## Discussion

Your driver extension calls this method to set properties on the HBA. The `properties` directory can contain the following keys:

- kIOPropertyVendorNameKey

- kIOPropertyProductNameKey

- kIOPropertyProductRevisionLevelKey

- kIOPropertyPortDescriptionKey

- kIOPropertyPortSpeedKey

- kIOPropertyPortTopologyKey

- kIOPropertySCSIParallelSignalingTypeKey

- kIOPropertyFibreChannelCableDescriptionKey

- kIOPropertyFibreChannelNodeWorldWideNameKey

- kIOPropertyFibreChannelPortWorldWideNameKey

- kIOPropertyFibreChannelAddressIdentifierKey

- kIOPropertyFibreChannelALPAKey

- kIOPropertySASAddressKey

The value of each property should be a pointer to a valid OSString object that represents the value for the property. The value must be of the proper type and size for the specified key.

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

UserRemoveHBAProperties

Removes properties from a host bus adapter in response to a call from the framework.

UserReportHBAConstraints

Reports the I/O constraints for this controller.

