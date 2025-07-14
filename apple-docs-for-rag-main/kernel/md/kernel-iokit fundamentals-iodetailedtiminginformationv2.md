

- Kernel
- IOKit Fundamentals
-  IODetailedTimingInformationV2 

Type Alias

# IODetailedTimingInformationV2

macOS 10.1+

``` source
typedef struct IODetailedTimingInformationV2 IODetailedTimingInformationV2;
```

## Topics

### Instance Properties

horizontalActive

Pixel clocks per line.

horizontalBlanking

Blanking clocks per line.

horizontalBorderLeft

Number of pixels in left horizontal border.

horizontalBorderRight

Number of pixels in right horizontal border.

horizontalScaled

If the mode is scaled, sets the size of the image before scaling or rotation.

horizontalScaledInset

If the mode is scaled, sets the number of active pixels to remove the left and right edges in order to display an underscanned image.

horizontalSyncConfig

kIOSyncPositivePolarity for positive polarity horizontal sync (0 for negative).

horizontalSyncLevel

Zero.

horizontalSyncOffset

First clock of horizontal sync.

horizontalSyncPulseWidth

Width of horizontal sync.

maxPixelClock

Maximum pixel clock frequency in Hz, with error.

minPixelClock

Minimum pixel clock frequency in Hz, with error.

numLinks

number of links to be used by a dual link timing, if zero, assume one link.

pixelClock

Pixel clock frequency in Hz.

scalerFlags

If the mode is scaled, kIOScaleStretchToFit may be set to allow stretching. kIOScaleRotateFlags is mask which may have the value given by kIOScaleRotate90, kIOScaleRotate180, kIOScaleRotate270 to display a rotated framebuffer.

signalConfig

kIOAnalogSetupExpected set if display expects a blank-to-black setup or pedestal. See VESA signal standards.

signalLevels

One of:

verticalActive

Number of lines per frame.

verticalBlanking

Blanking lines per frame.

verticalBorderBottom

Number of lines in bottom vertical border.

verticalBorderTop

Number of lines in top vertical border.

verticalScaled

If the mode is scaled, sets the size of the image before scaling or rotation.

verticalScaledInset

If the mode is scaled, sets the number of active lines to remove the top and bottom edges in order to display an underscanned image.

verticalSyncConfig

kIOSyncPositivePolarity for positive polarity vertical sync (0 for negative).

verticalSyncLevel

Zero.

verticalSyncOffset

First line of vertical sync.

verticalSyncPulseWidth

Height of vertical sync.

bitsPerColorComponent

colorimetry

dscCompressedBitsPerPixel

dscSliceHeight

dscSliceWidth

dynamicRange

pixelEncoding

verticalBlankingExtension

verticalBlankingMaxShrinkPerFrame

verticalBlankingMaxStretchPerFrame

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

