

- Kernel
- Hardware Families
- Graphics and Displays
- IOFramebuffer
-  setGammaTable 

# setGammaTable

Set the gamma table to be used by the framebuffer.

``` source
virtual IOReturn setGammaTable(
 UInt32channelCount,
 UInt32dataCount, 
 UInt32dataWidth,
 void *data ); 
```

## Parameters 

`channelCount`  

Defines the number of channels in the supplied data. macOS will pass three for separate R, G, B data, or one if the same data should apply to all channels.

`dataCount`  

The number of data entries per channel.

`dataWidth`  

The number of bits in each entry. 8 for OS X 10.1 and earlier, 16 for later releases.

`data`  

The packed array of correction data. Data is passed for the R (or single) channel followed by the G & B channels. Each entry is one or two bytes (if dataWidth \> 8).

## Return Value

an IOReturn code.

## Overview

IOFramebuffer subclasses should implement this method to allow a gamma table to be set.

## See Also

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

