

- Core Graphics
- Quartz Window Services
-  Window List Option Constants 

API Collection

# Window List Option Constants

Specifies which windows in the current user session to include in a generated list.

## Overview

The optionIncludingWindow and excludeDesktopElements constants may be combined with the other constants by adding (or ORing) them together and passing the resulting value to the appropriate function.

These constants let you retrieve windows in the current user session only. You cannot use them to retrieve windows from other active user sessions running on the system.

## Topics

### Constants

static var optionAll: CGWindowListOption

static var optionOnScreenOnly: CGWindowListOption

static var optionOnScreenAboveWindow: CGWindowListOption

static var optionOnScreenBelowWindow: CGWindowListOption

static var optionIncludingWindow: CGWindowListOption

static var excludeDesktopElements: CGWindowListOption

## See Also

### Constants

Window Sharing Constants

Specifies whether and how windows are shared between applications.

Backing Store Types

Specifies how the window device buffers drawing commands.

Window Image Types

Specifies the options for capturing an image of a window.

CGWindowID Encoding Type

Defines the encoding type for window IDs.

Null Window

Defines a guaranteed invalid window ID.

Window Sharing Encoding Type

Defines the encoding type for window sharing values.

Window Backing Encoding Type

Defines the encoding type for window backing types.

Required Window List Keys

The keys that are guaranteed to be available in a window’s information dictionary.

Optional Window List Keys

The keys that may optionally be available inside a window’s information dictionary.

