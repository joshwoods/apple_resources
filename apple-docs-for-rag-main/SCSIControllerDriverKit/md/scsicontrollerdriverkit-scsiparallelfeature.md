

- SCSIControllerDriverKit
-  SCSIParallelFeature 

Enumeration

# SCSIParallelFeature

A feature that the driver extension supports.

DriverKit

``` source
typedef enum SCSIParallelFeature : unsigned int { ... } SCSIParallelFeature;
```

## Overview

This enumeration defines feature selectors the framework uses to identify features of the SCSI parallel interface. The UserDoesHBASupportSCSIParallelFeature function uses these to report whether the HBA supports a SCSI parallel interface feature. The framework also uses these to request negotiation and report negotiation results between the controller and the device.

## Topics

### Feature selectors

kSCSIParallelFeature_WideDataTransfer

The selector for support of wide data transfers.

kSCSIParallelFeature_SynchronousDataTransfer

The selector for support of synchronous data transfers.

kSCSIParallelFeature_QuickArbitrationAndSelection

The selector for support of quick arbitration and selection (QAS).

kSCSIParallelFeature_DoubleTransitionDataTransfers

The selector for support of double transition (DT) data transfers.

kSCSIParallelFeature_InformationUnitTransfers

The selector for SPI information unit (IU) transfers.

kSCSIParallelFeature_TotalFeatureCount

The total number of supported features.

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

UserMapHBAData

Maps any host bus adapter (HBA)-specific task data in response to a call from the framework.

UserSetHBAProperties

Sets multiple properties for a host bus adapter.

UserRemoveHBAProperties

Removes properties from a host bus adapter in response to a call from the framework.

UserReportHBAConstraints

Reports the I/O constraints for this controller.

