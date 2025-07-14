

- Kernel
- Hardware Families
- Graphics and Displays
-  IONDRVFramebuffer 

Class

# IONDRVFramebuffer

macOS 10.0+

``` source
class IONDRVFramebuffer : IOFramebuffer
```

## Topics

### Instance Methods

- checkDriver

- connectFlags

- createI2C

- displayI2CPower

- doControl

- doDriverIO

- doI2CRequest

- doStatus

- enableController

- findVRAM

- free

- getApertureRange

- getAppleSense

- getAttribute

- getAttributeForConnection

- getConnectionCount

- getCurrentConfiguration

- getCurrentDisplayMode

- getDDCBlock

- getDisplayModeCount

- getDisplayModes

- getInformationForDisplayMode

- getMetaClass

- getOnlineState

- getPixelFormats

- getPixelFormatsForDisplayMode

- getPixelInformation

- getResInfoForArbMode

- getResInfoForDetailed

- getResInfoForMode

- getStartupDisplayMode

- getTimingInfoForDisplayMode

- getVRAMRange

- hasDDCConnect

- initForPM

- initialPowerStateForDomainState

- isConsoleDevice

- iterateAllModes

- makeSubRange

- mapDepthIndex

- maxCapabilityForDomainState

- ndrvGetSetFeature

- ndrvSetDisplayPowerState

- ndrvSetPowerState

- ndrvUpdatePowerState

- powerStateForDomainState

- probe

- processConnectChange

- registerForInterruptType

- requestProbe

- searchOfflineMode

- setApertureEnable

- setAttribute

- setAttributeForConnection

- setCLUTWithEntries

- setConnectionFlags

- setCursorImage

- setCursorState

- setDetailedTiming

- setDetailedTimings

- setDisplayMode

- setGammaTable

- setInfoProperties

- setInterruptState

- setMirror

- setProperties

- setStartupDisplayMode

- setupForCurrentConfig

- start

- stop

- undefinedSymbolHandler

- unregisterInterrupt

- validateDetailedTiming

- validateDisplayMode

### Type Methods

+ VSLDisposeInterruptService

+ VSLDoInterruptService

+ VSLNewInterruptService

+ VSLPrepareCursorForHardwareCursor

+ extControl

+ extStatus

## Relationships

### Inherits From

- IOFramebuffer

## See Also

### Devices

IOFramebuffer

The base class for graphics devices to be made available as part of the desktop.

IOGraphicsDevice

IOFBCursorControlAttribute

IOFBCursorControlCallouts

IOTVector

