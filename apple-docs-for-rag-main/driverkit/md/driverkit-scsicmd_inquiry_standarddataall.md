

- DriverKit
-  SCSICmd_INQUIRY_StandardDataAll 

Structure

# SCSICmd_INQUIRY_StandardDataAll

DriverKitiOSiPadOSmacOS

``` source
typedef struct SCSICmd_INQUIRY_StandardDataAll { ... } SCSICmd_INQUIRY_StandardDataAll;
```

## Overview

This structure defines the all of the fields that can be returned in repsonse to the INQUIRy request for the standard data. There is no requirement as to how much of the additional data must be returned by a device.

## Topics

### Instance Properties

ADDITIONAL_LENGTH

PERIPHERAL_DEVICE_TYPE

PRODUCT_IDENTIFICATION

PRODUCT_REVISION_LEVEL

RESPONSE_DATA_FORMAT

RMB

Reserved1

Reserved2

SCCSReserved

VENDOR_IDENTIFICATION

VERSION

VERSION_DESCRIPTOR

VendorSpecific1

VendorSpecific2

flags1

flags2

flags3

## See Also

### Structures

IODMACommandSpecification

IOHistogramReportValues

IOHistogramSegmentConfig

IONormDistReportValues

IORPCMessageErrorReturnContent

IOReportChannel

IOReportChannelList

IOReportChannelType

IOReportElement

IOReportElementValues

IOReportInterest

IOReportInterestList

IOSimpleArrayReportValues

IOSimpleReportValues

IOStateReportValues

