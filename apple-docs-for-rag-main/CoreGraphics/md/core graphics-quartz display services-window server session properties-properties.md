

- Core Graphics
- Quartz Display Services
-  Window Server Session Properties 

API Collection

# Window Server Session Properties

The keys for the standard properties in a window server session dictionary.

## Overview

To learn how to use these keys to access the values in a session dictionary, see CFDictionary.

## Topics

### Constants

var kCGSessionUserIDKey: String

A `CFNumber` 32-bit unsigned integer value that encodes a user ID for the session’s current user.

var kCGSessionUserNameKey: String

A `CFString` value that encodes the session’s short user name as set by the login operation.

var kCGSessionConsoleSetKey: String

A `CFNumber` 32-bit unsigned integer value that represents a set of hardware composing a console.

var kCGSessionOnConsoleKey: String

A `CFBoolean` value indicating whether the session is on a console.

var kCGSessionLoginDoneKey: String

A `CFBoolean` value indicating whether the login operation has been done.

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

enum CGDisplayStreamUpdateRectType

Use these constants to determine which rectangles your app is interested in.

enum CGDisplayStreamFrameStatus

Describes a frame update event.

Display Stream Optional Property Keys

These keys are used to populate the `properties` dictionary used when creating a new display stream.

Display Stream YCbCr to RGB conversion Matrix Options

These strings are used to specify a matrix for the yCbCrMatrix option.

