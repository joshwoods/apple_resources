

- Core Graphics
- Quartz Display Services
-  Display Fade Blend Fractions 

API Collection

# Display Fade Blend Fractions

The lower and upper bounds for blend color fractions during a display fade operation.

## Overview

For general information about blend fractions, see the data type CGDisplayBlendFraction. For information about how these constants are used, see the function CGDisplayFade(_:_:_:_:_:_:_:_:).

## Topics

### Constants

var kCGDisplayBlendNormal: Double

The blend color is not applied at the start or end of a fade operation.

var kCGDisplayBlendSolidColor: Double

The user sees only the blend color at the start or end of a fade operation.

## See Also

### Constants

struct CGCaptureOptions

Configuration parameters that are used when capturing displays.

struct CGDisplayChangeSummaryFlags

The configuration parameters that are passed to a display reconfiguration callback function.

struct CGConfigureOption

The scope of the changes in a display configuration transaction.

Display Fade Constants

Values relating to fade operations.

Display ID Defaults

Default values for a display ID.

Display Mode Standard Properties

Keys for the standard properties in a display mode dictionary.

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

