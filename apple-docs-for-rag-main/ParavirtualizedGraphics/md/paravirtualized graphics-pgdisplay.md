

- Paravirtualized Graphics
-  PGDisplay 

Protocol

# PGDisplay

An object that provides display functionality to the guest operating system in a way that the host-side virtual machine app can intercept.

Mac Catalyst 14.0+macOS 11.0+

``` source
protocol PGDisplay : NSObjectProtocol
```

## Overview

The framework emulates hot-plugging to the display. After you create the display object, set the modeList property to a list of modes you want the display to use. The first time you set the mode list, the framework connects the display to the virtualized graphics card. When you release the display object, the device simulates unplugging the display.

## Topics

### Setting Display Modes

var modeList: [PGDisplayMode]

The list of display modes that the virtual display supports.

**Required**

### Getting the Guest Cursor Position

var cursorPosition: PGDisplayCoord_t

The current cursor location in the guest environment.

**Required**

### Handling Frame Updates

var guestPresentCount: Int

The number of frame presents that the guest has generated since object creation.

**Required**

var hostPresentCount: Int

The number of unique frames that the host has encoded since object creation.

**Required**

var minimumTextureUsage: MTLTextureUsage

The Metal texture usage flags necessary for any texture that can be a destination for frame data.

**Required**

func encodeCurrentFrame(to: any MTLCommandBuffer, texture: any MTLTexture, region: MTLRegion) -> Bool

Encodes Metal commands to process the current frame and write it to a texture.

**Required**

### Inspecting Display Properties

var name: String?

The display’s name that you specified at creation time.

**Required**

var serialNum: UInt32

The display’s serial number that you specified at creation time.

**Required**

var port: Int

The display’s accelerator port that you specified at creation time.

**Required**

var sizeInMillimeters: NSSize

The display’s virtual dimensions, in millimeters, that you specified at creation time.

**Required**

### Inspecting the Display Handlers

var queue: dispatch_queue_t?

The queue that the framework uses when dispatching messages to any of the display’s registered handlers.

**Required**

var cursorGlyphHandler: PGDisplayCursorGlyphHandler?

A handler that the framework calls to change the cursor’s appearance.

**Required**

var cursorShowHandler: PGDisplayCursorShowHandler?

A handler that the framework calls to change the cursor’s visibility.

**Required**

var modeChangeHandler: PGDisplayModeChangeHandler?

A handler that the framework calls to change the virtual display’s graphics mode.

**Required**

var newFrameEventHandler: PGDisplayNewFrameEventHandler?

A handler that the framework calls when the guest environment has a new frame to display.

**Required**

### Instance Properties

var cursorMoveHandler: PGDisplayCursorMoveHandler?

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Displays

class PGDisplayDescriptor

A descriptor for a virtual display.

class PGDisplayMode

A description of a supported display mode.

struct PGDisplayCoord_t

Coordinates that describe sizes or offsets within a 2D array of pixels.

