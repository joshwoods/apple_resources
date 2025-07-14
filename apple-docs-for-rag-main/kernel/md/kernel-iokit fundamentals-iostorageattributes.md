

- Kernel
- IOKit Fundamentals
-  IOStorageAttributes 

# IOStorageAttributes

macOS 10.6+

``` source
struct IOStorageAttributes {
    ...
};
```

## Discussion

Attributes of read and write storage requests.

## Topics

### Fields

options

Options for the request. See IOStorageOptions.

bufattr

Reserved for future use. Set to zero.

### Instance Properties

priority

reserved0024

reserved0032

reserved0064

adjustedOffset

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

IODisplayModeInformation

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

