

- Kernel
- IOKit Fundamentals
-  IODebuggerRxHandler 

Type Alias

# IODebuggerRxHandler

macOS 10.0+

``` source
typedef void (*IODebuggerRxHandler)(IOService *target, void *buffer, UInt32 *length, UInt32 timeout);
```

## Parameters 

`target`  

The target object.

`buffer`  

KDP receive buffer. The buffer allocated has room for 1518 bytes. The receive handler must not overflow this buffer.

`length`  

The amount of data received and placed into the buffer. Set to 0 if no frame was received during the poll interval.

`timeout`  

The amount of time to poll in milliseconds while waiting for a frame to arrive.

## Discussion

Defines the receive handler that must be implemented by the target to service KDP receive requests. This handler is called by kdpReceiveDispatcher().

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

