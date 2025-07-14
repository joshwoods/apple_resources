

- Kernel
- Hardware Families
-  Graphics and Displays 

API Collection

# Graphics and Displays

Implement a driver that interacts with graphics and video hardware.

## Topics

### Interfaces

IODisplayConnect

IOBacklightDisplay

IODisplay

IODisplayParameterHandler

IOAccelerator

### Video

IOVideoDevice

A class that represents a video device.

IONVRAMController

IOVideoControlDictionary

IOVideoStream

A class representing a stream of video data buffers passed from kernel to user space and back again.

IOVideoStreamDictionary

IOVideoStreamFormatDictionary

### Devices

IONDRVFramebuffer

IOFramebuffer

The base class for graphics devices to be made available as part of the desktop.

IOGraphicsDevice

IOFBCursorControlAttribute

IOFBCursorControlCallouts

IOTVector

### User-Space Access

IOVideoDeviceUserClient

IOVideoDeviceUserClientInit

### Blit Structures

IOBlitCopyRectangle

IOBlitCopyRectangles

IOBlitCopyRegion

IOBlitCursor

IOBlitMemory

IOBlitMemoryRef

IOBlitOperation

IOBlitRectangle

IOBlitRectangles

IOBlitScanlines

IOBlitSourceType

IOBlitSurface

IOBlitType

IOBlitVertex

IOBlitVertices

### Framebuffer Utilities

agdcGTraceToken

VSLDisposeInterruptService

VSLDoInterruptService

VSLNewInterruptService

VSLPrepareCursorForHardwareCursor

### Display Keys

gIODisplayAmbientLightSensorKey

gIODisplayAudioBalanceLRKey

gIODisplayAudioBassKey

gIODisplayAudioMuteAndScreenBlankKey

gIODisplayAudioProcessorModeKey

gIODisplayAudioTrebleKey

gIODisplayBlueGammaScaleKey

gIODisplayBrightnessFadeKey

gIODisplayBrightnessKey

gIODisplayBrightnessProbeKey

gIODisplayCapabilityStringKey

gIODisplayContrastKey

gIODisplayControllerIDKey

gIODisplayFadeStyle

gIODisplayFadeStyleKey

gIODisplayFadeTime1

gIODisplayFadeTime1Key

gIODisplayFadeTime2

gIODisplayFadeTime2Key

gIODisplayFadeTime3

gIODisplayFadeTime3Key

gIODisplayFirmwareLevelKey

gIODisplayGUIDKey

gIODisplayGammaScaleKey

gIODisplayGreenGammaScaleKey

gIODisplayHorizontalPositionKey

gIODisplayHorizontalSizeKey

gIODisplayLinearBrightnessKey

gIODisplayLinearBrightnessProbeKey

gIODisplayMCCSVersionKey

gIODisplayManufacturerSpecificKey

gIODisplayMaxValueKey

gIODisplayMicrophoneVolumeKey

gIODisplayMinValueKey

gIODisplayOverscanKey

gIODisplayParallelogramKey

gIODisplayParametersCommitKey

gIODisplayParametersDefaultKey

gIODisplayParametersFlushKey

gIODisplayParametersKey

gIODisplayParametersTheatreModeKey

gIODisplayParametersTheatreModeWindowKey

gIODisplayPincushionKey

gIODisplayPowerModeKey

gIODisplayPowerStateKey

gIODisplayRedGammaScaleKey

gIODisplayRotationKey

gIODisplaySelectedColorModeKey

gIODisplaySpeakerSelectKey

gIODisplaySpeakerVolumeKey

gIODisplayTechnologyTypeKey

gIODisplayTrapezoidKey

gIODisplayUsableLinearBrightnessKey

gIODisplayUsageTimeKey

gIODisplayValueKey

gIODisplayVerticalPositionKey

gIODisplayVerticalSizeKey

gIODisplayVideoBestKey

### Additional Types

VDClutBehavior

VDClutBehaviorPtr

VDCommunicationInfoPtr

VDCommunicationInfoRec

VDCommunicationPtr

VDCommunicationRec

VDConfigurationFeatureListRec

VDConfigurationFeatureListRecPtr

VDConfigurationPtr

VDConfigurationRec

VDConvolutionInfoPtr

VDConvolutionInfoRec

VDDDCBlockPtr

VDDDCBlockRec

VDDefMode

VDDefModePtr

VDDetailedTimingPtr

VDDetailedTimingRec

VDDisplayConnectInfoPtr

VDDisplayConnectInfoRec

VDDisplayTimingRangePtr

VDDisplayTimingRangeRec

VDDrawHardwareCursorPtr

VDDrawHardwareCursorRec

VDEntRecPtr

VDEntryRecord

VDFlagRecPtr

VDFlagRecord

VDGamRecPtr

Represents a type used by the Video Components API.

VDGammaInfoPtr

VDGammaInfoRec

VDGammaRecord

VDGetGammaListPtr

VDGetGammaListRec

VDGrayPtr

VDGrayRecord

VDHardwareCursorDrawStatePtr

VDHardwareCursorDrawStateRec

VDMirrorPtr

VDMirrorRec

VDMultiConnectInfoPtr

VDMultiConnectInfoRec

VDPageInfo

VDPgInfoPtr

VDPowerStatePtr

VDPowerStateRec

VDPrivateSelectorDataRec

VDPrivateSelectorRec

VDResolutionInfoPtr

VDResolutionInfoRec

VDRetrieveGammaPtr

VDRetrieveGammaRec

VDScalerInfoPtr

VDScalerInfoRec

VDScalerPtr

VDScalerRec

VDSetEntryPtr

VDSetEntryRecord

VDSetHardwareCursorPtr

VDSetHardwareCursorRec

VDSettings

VDSettingsPtr

VDSizeInfo

VDSupportsHardwareCursorPtr

VDSupportsHardwareCursorRec

VDSwitchInfoPtr

VDSwitchInfoRec

VDSyncInfoPtr

VDSyncInfoRec

VDSzInfoPtr

VDTimingInfoPtr

VDTimingInfoRec

VDVideoParametersInfoPtr

VDVideoParametersInfoRec

## See Also

### Interfaces

Audio

Implement a driver that interacts with audio hardware.

HID

Implement a driver that interacts with human interface devices, such as mice and keyboards.

Network

Implement a driver that interacts with network interfaces such as Ethernet adaptors.

SCSI

Implement a driver that supports Small Computer System Interface (SCSI) protocols.

Mass Storage

Implement a driver that communicates with CD, DVD, or other mass storage devices.

