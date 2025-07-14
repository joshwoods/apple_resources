

- Core Graphics
- Quartz Display Services
-  Display Mode Standard Properties 

API Collection

# Display Mode Standard Properties

Keys for the standard properties in a display mode dictionary.

## Overview

To learn how to use these keys to access the values in a display mode dictionary, see CFDictionary.

### Special Considerations

Starting in OS X v10.6, display mode dictionaries have been made obsolete by the display mode opaque type. For more information on display modes, seeChanging Display Modes (OS X v10.6 or later).

## Topics

### Constants

var kCGDisplayWidth: String

Specifies a CFNumber integer value that represents the width of the display in pixels.

Deprecated

var kCGDisplayHeight: String

Specifies a CFNumber integer value that represents the height of the display in pixels.

var kCGDisplayMode: String

Specifies a `CFNumber` integer value that represents the I/O Kit display mode number.

var kCGDisplayBitsPerPixel: String

Specifies a CFNumber integer value that represents the number of bits in a pixel.

var kCGDisplayBitsPerSample: String

Specifies a CFNumber integer value that represents the number of bits in an individual sample (for example, a color value in an RGB pixel).

var kCGDisplaySamplesPerPixel: String

Specifies a CFNumber integer value that represents the number of samples in a pixel.

var kCGDisplayRefreshRate: String

Specifies a `CFNumber` double-precision floating point value that represents the refresh rate of a CRT display.

var kCGDisplayModeUsableForDesktopGUI: String

Specifies a CFBoolean value that indicates whether the display is suitable for use with the macOS graphical user interface. The criteria include factors such as sufficient width and height and adequate pixel depth.

var kCGDisplayIOFlags: String

Specifies a CFNumber integer value that contains the I/O Kit display mode flags. For more information, see the header file `IOKit/IOGraphicsTypes.h`.

var kCGDisplayBytesPerRow: String

Specifies a CFNumber integer value that represents the number of bytes in a row on the display.

## See Also

### Constants

struct CGCaptureOptions

Configuration parameters that are used when capturing displays.

struct CGDisplayChangeSummaryFlags

The configuration parameters that are passed to a display reconfiguration callback function.

struct CGConfigureOption

The scope of the changes in a display configuration transaction.

Display Fade Blend Fractions

The lower and upper bounds for blend color fractions during a display fade operation.

Display Fade Constants

Values relating to fade operations.

Display ID Defaults

Default values for a display ID.

Display Mode Optional Properties

Keys for optional properties in a display mode dictionary.

Reserved Window Levels

Window level constants.

struct CGScreenUpdateOperation

Types of screen-update operations.

enum CGWindowLevelKey

Keys that represent the standard window levels in macOS. Quartz includes these keys to support application frameworks like Cocoa. Applications do not need to use them directly.

Window Server Session Properties

The keys for the standard properties in a window server session dictionary.

enum CGDisplayStreamUpdateRectType

Use these constants to determine which rectangles your app is interested in.

enum CGDisplayStreamFrameStatus

Describes a frame update event.

Display Stream Optional Property Keys

These keys are used to populate the `properties` dictionary used when creating a new display stream.

Display Stream YCbCr to RGB conversion Matrix Options

These strings are used to specify a matrix for the yCbCrMatrix option.

