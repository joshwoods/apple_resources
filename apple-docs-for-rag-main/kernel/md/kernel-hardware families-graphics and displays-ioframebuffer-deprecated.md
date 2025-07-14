

- Kernel
- Hardware Families
- Graphics and Displays
-  IOFramebuffer Deprecated

Class

# IOFramebuffer

The base class for graphics devices to be made available as part of the desktop.

macOS 10.0+

``` source
class IOFramebuffer : IOGraphicsDevice
```

Deprecated

The IOFramebuffer class only enables simple framebuffer operation, which is not sufficient for the full macOS user experience. This class is not intended for use by third-party device drivers and is documented for informational purposes only.

## Overview

The IOFramebuffer base class defines APIs used to publish a linear framebuffer device. Device driver writers should subclass this class to provide a X native driver. macOS will also utilize 'ndrv' drivers via a subclass of IOFramebuffer IONDRVFramebuffer that does not require device driver writers to provide a X native driver.

There are no in kernel clients of IOFramebuffer aside from rudimentary console and panic UI supported by the IOFramebuffer class. The IOFramebuffer class provides the IOUserClient implementation to allow the CoreGraphics server to provide the user accessible interface to all displays on a macOS system, and this is further layered underneath application frameworks. Device driver writers should not need any knowledge of this part of the interfaces. Similarly the instance variables of IOFramebuffer are mostly used for cursor rendering which is handled by the IOFramebuffer class, and should be avoided by subclass implementors. Only IOFramebuffer methods with header documentation in this header are designed for subclasses to implement.

IOFramebuffer provides simple framebuffer operation - acceleration for 2D, 3D and video may be provided by a separate implementation of the IOAccelerator class.

## Topics

### Miscellaneous

connectFlags

Return display sense information for legacy Apple sensing.

convertCursorImage

Utility method of IOFramebuffer to convert cursor image to a hardware cursor format.

doI2CRequest

Carry out an I2C request.

enableController

Perform first time setup of the framebuffer.

flushCursor

Perform any needed cache flushing after software cursor rendering.

getApertureRange

Return reference to IODeviceMemory object representing memory range of framebuffer.

getAppleSense

Return display sense information for legacy Apple sensing.

getAttribute

Generic method to retrieve some attribute of the framebuffer device.

getAttributeForConnection

Generic method to retrieve some attribute of the framebuffer device, specific to one display connection.

getConnectionCount

Reports the number of display connections the device supports, driven from one framebuffer.

getCurrentDisplayMode(IODisplayModeID *, IOIndex *)

Return the framebuffers display mode and depth to be used during boot and at startup.

getDDCBlock

Return display EDID data.

getDisplayModeCount

Return the number of display modes the framebuffer supports.

getDisplayModes

Return the number of display modes the framebuffer supports.

getInformationForDisplayMode

Return information about a given display mode.

getPixelFormats

List the pixel formats the framebuffer supports.

getPixelFormatsForDisplayMode

Obsolete.

getPixelInformation

Return information about the framebuffer format for a given display mode and depth.

getStartupDisplayMode

Return the framebuffers display mode and depth to be used during boot and at startup.

getTimingInfoForDisplayMode

Returns a timing description for a display mode.

getVRAMRange

Return reference to IODeviceMemory object representing memory range of all the cards vram.

handleEvent

Notify IOFramebuffer superclass code of events.

hasDDCConnect

Return display DDC connect state.

readDDCClock

Reads the input state of the I2C clock line on a bus.

readDDCData

Reads the input state of the I2C data line on a bus.

registerForInterruptType

Set callbacks for driver to call on interrupt events.

setApertureEnable

Enable an aperture on the framebuffer (usually unimplemented, no OS usage).

setAttribute

Generic method to set some attribute of the framebuffer device.

setAttributeForConnection

Generic method to set some attribute of the framebuffer device, specific to one display connection.

setCLUTWithEntries

Set the color lookup table to be used by the framebuffer in indexed modes.

setCurrentDisplayMode

Set the framebuffers current display mode and depth.

setCursorImage

Set a new image for the hardware cursor.

setCursorState

Set a new position and visibility for the hardware cursor.

setDDCClock

Sets the state of the I2C clock line on a bus.

setDDCData

Sets the state of the I2C data line on a bus.

setDetailedTimings

Installs an array of OS programmed detailed timings to be made available by the driver.

setDisplayMode

Set the framebuffers current display mode and depth.

setGammaTable

Set the gamma table to be used by the framebuffer.

setInterruptState

Enable or disable a callback previously installed by registerForInterruptType().

setStartupDisplayMode

Set the framebuffers display mode and depth to be used during boot and at startup.

unregisterInterrupt(void *)

Remove a callback previously installed by registerForInterruptType().

unregisterInterrupt(void *, UInt32)

Enable or disable a callback previously installed by registerForInterruptType().

validateDetailedTiming

Reports whether a detailed timing is able to be programmed with the device.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- addFramebufferNotification

- addFramebufferNotificationWithOptions

- attach

- callPlatformFunction

- close

- connectFlags

- convertCursorImage

- deliverFramebufferNotification

- diagnoseReport

- didTerminate

- doI2CRequest

- enableController

- enableDDCRaster

- flushCursor

- free

- getAggressiveness

- getApertureRange

- getAppleSense

- getAttribute

- getAttributeExt

- getAttributeForConnection

- getAttributeForConnectionExt

- getBoundingRect

- getConnectionCount

- getControllerWorkLoop

- getCurrentDisplayMode

- getDDCBlock

- getDisplayModeCount

- getDisplayModes

- getGraphicsSystemWorkLoop

- getInformationForDisplayMode

- getMetaClass

- getNotificationSemaphore

- getPixelFormats

- getPixelFormatsForDisplayMode

- getPixelInformation

- getStartupDisplayMode

- getTimingInfoForDisplayMode

- getVBLTime

- getVRAMRange

- getWorkLoop

- handleEvent

- hasDDCConnect

- hideCursor

- isConsoleDevice

- message

- moveCursor

- newUserClient

- open

- powerStateDidChangeTo

- powerStateWillChangeTo

- readDDCClock

- readDDCData

- registerForInterruptType

- requestProbe

- requestTerminate

- resetCursor

- resetLimitState

- sendLimitState

- serializeInfo

- setAggressiveness

- setApertureEnable

- setAttribute

- setAttributeExt

- setAttributeForConnection

- setAttributeForConnectionExt

- setBackingFramebuffer

- setCLUTWithEntries

- setCursorImage

- setCursorState

- setDDCClock

- setDDCData

- setDetailedTimings

- setDisplayMode

- setGammaTable

- setInterruptState

- setNumber

- setPowerState

- setProperties

- setStartupDisplayMode

- setupForCurrentConfig

- showCursor

- start

- stop

- switchBackingFramebuffer

- terminate

- unregisterInterrupt

- validateDetailedTiming

- willTerminate

### Type Methods

+ handleVBL

+ initialize

## Relationships

### Inherits From

- IOGraphicsDevice

## See Also

### Devices

IONDRVFramebuffer

IOGraphicsDevice

IOFBCursorControlAttribute

IOFBCursorControlCallouts

IOTVector

