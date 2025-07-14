

- Kernel
- IOKit Fundamentals
-  IODisplayModeInformation 

Type Alias

# IODisplayModeInformation

macOS 10.0+

``` source
typedef struct IODisplayModeInformation IODisplayModeInformation;
```

## Topics

### Instance Properties

flags

Flags for the mode, including:

imageHeight

Physical height of active image if known, in millimeters, otherwise zero.

imageWidth

Physical width of active image if known, in millimeters, otherwise zero.

maxDepthIndex

Highest depth index available in this display mode.

nominalHeight

Number of visible pixel rows.

nominalWidth

Number of pixels visible per row.

refreshRate

Refresh rate in fixed point 16.16.

reserved

Set to zero.

## See Also

### Common Types

IOAccelBounds

IOAccelDeviceRegion

IOAccelID

IOAccelSize

IOAccelSurfaceInformation

IOAccelSurfaceReadData

IOAccelSurfaceScaling

IOAddressRange

IOAddressSegment

IOAlignment

IOAppleTimingID

IOAsyncMethod

IOBlockStorageDeviceExtent

Extent for unmap storage requests.

IOBlockStorageProvisionDeviceExtent

IOByteCount

IOByteCount32

IOByteCount64

IOCSRKeyType

IOCacheMode

IOColorComponent

IOColorEntry

IOCommandCode

IOCommandID

IOCommandKind

IOConfigKeyType

IODMAMapPageList

IODMAMapSpecification

IODTCompareAddressCellFunc

IODTNVLocationFunc

IODataQueueClientDequeueEntryBlock

IODataQueueClientEnqueueEntryBlock

IODebuggerLinkStatusHandler

IODebuggerRxHandler

IODebuggerSetModeHandler

IODebuggerTxHandler

IODetailedTimingInformation

IODetailedTimingInformationV1

IODetailedTimingInformationV2

IODispatchBlock

IODispatchFunction

IODispatchLogFunction

IODispatchQueueCancelHandler

IODispatchQueueName

IODispatchSourceCancelHandler

IODisplayModeID

IODisplayProductID

IODisplayScalerInformation

IODisplayTimingRange

IODisplayTimingRangeV1

IODisplayTimingRangeV2

IODisplayVendorID

IOEnetMulticastMode

IOEnetPromiscuousMode

IOEthernetAddress

IOExternalAsyncMethod

IOExternalMethod

IOExternalMethodAction

IOExternalMethodArguments

IOExternalMethodDispatch

IOExternalTrap

IOFBCursorRef

IOFBDPLinkConfig

IOFBDisplayModeDescription

IOFBHDRMetaData

IOFBHDRMetaDataV1

IOFBInterruptProc

IOFixed

IOFixed1616

IOFixedPoint32

IOFourCharCode

IOFramebufferNotificationHandler

IOFramebufferNotificationNotify

IOGBounds

IOGPoint

IOGSize

IOHardwareCursorDescriptor

IOHardwareCursorInfo

IOIndex

IOInterruptAction

IOInterruptActionBlock

IOInterruptDispatchSourcePayload

IOInterruptHandler

IOInterruptState

IOInterruptVectorNumber

IOItemCount

IOLock

IOLogicalAddress

IOMediaAttributeMask

IOMediaState

IOMessage

IOMethod

IONDRVControlParameters

IONVRAMDescriptor

IONamedValue

IONotificationRef

IOOptionBits

IOOutputAction

IOPCIDeviceConfigHandler

IOPCIEvent

IOPCIPhysicalAddress

IOPMCalendarStruct

IOPMDriverAssertionID

IOPMDriverAssertionLevel

IOPMDriverAssertionType

IOPMSettingControllerCallback

IOPhysicalAddress

IOPhysicalAddress32

IOPhysicalAddress64

IOPhysicalLength

IOPhysicalLength32

IOPhysicalLength64

IOPhysicalRange

IOPixelAperture

IOPixelEncoding

IOPixelInformation

IOPowerStateChangeNotification

IOPropertyName

IORPC

IORPCMessage

IORPCMessageErrorReturn

IORPCMessageErrorReturnContent

IORPCMessageMach

IORWLock

IORangeScalar

IORecursiveLock

IORegistryEntryApplierFunction

IORegistryPlaneName

IOReportCategories

IOReportConfigureAction

IOReportFormat

IOReportQuantity

IOReportScaleFactor

IOReportUnit

IOReportUnits

IOReportUpdateAction

IOReturn

IOSelect

IOService

IOServiceApplierFunction

IOServiceInterestContent64

IOServiceInterestHandler

IOServiceInterestHandlerBlock

IOServiceMatchingNotificationHandler

IOServiceMatchingNotificationHandlerBlock

IOServiceName

IOServiceNotificationBlock

IOServiceNotificationHandler

IOSimpleLock

IOStorageAccess

IOStorageAttributes

IOStorageCompletion

IOStorageCompletionAction

IOStorageExtent

IOStorageGetProvisionStatusOptions

IOStorageOptions

IOStoragePriority

IOStorageProvisionExtent

IOStorageSynchronizeOptions

IOStorageUnmapOptions

IOStreamMode

IOThread

IOThreadFunc

IOTimeStampIntervalConstantFiltered

IOTimingInformation

IOTrackingCallSiteInfo

IOTrap

IOUserClientAsyncArgumentsArray

IOUserClientAsyncReferenceArray

IOUserClientMethodArguments

IOUserClientMethodDispatch

IOUserClientMethodFunction

IOUserClientScalarArray

IOVersion

IOVideoDeviceNotification

IOVideoDeviceNotificationMessage

IOVideoStreamDescription

IOVirtualAddress

IOVirtualRange

