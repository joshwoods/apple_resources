

- Kernel
- IOKit Fundamentals
-  IOPixelInformation 

Type Alias

# IOPixelInformation

macOS 10.0+

``` source
typedef struct IOPixelInformation IOPixelInformation;
```

## Topics

### Instance Properties

activeHeight

Number of visible pixel rows.

activeWidth

Number of pixels visible per row.

bitsPerComponent

Number of bits per component in each pixel.

bitsPerPixel

The number of bits per pixel, including unused bits and alpha.

bytesPerPlane

Not used.

bytesPerRow

The number of bytes per row.

componentCount

One for indexed pixels, three for direct pixel formats.

componentMasks

Mask of the bits valid for each component of the pixel - in R, G, B order for direct pixels.

flags

None defined - set to zero.

pixelFormat

String description of the pixel format - IO32BitDirectPixels, IO16BitDirectPixels etc.

pixelType

One of kIOCLUTPixels (indexed pixels with changeable CLUT), kIORGBDirectPixels (direct pixels).

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

