

- Core Graphics
-  Quartz Window Services 

API Collection

# Quartz Window Services

Provides information about the windows managed by the macOS window server.

## Overview

This includes the onscreen windows seen on the user’s desktop and any offscreen windows used by the running applications. You can also use Quartz Window Services to generate images based on the contents of windows.

## Topics

### Getting Window Information

func CGWindowListCopyWindowInfo(CGWindowListOption, CGWindowID) -> CFArray?

Generates and returns information about the selected windows in the current user session.

func CGWindowListCreateDescriptionFromArray(CFArray?) -> CFArray?

Generates and returns information about windows with the specified window IDs.

func CGWindowListCreateImage(CGRect, CGWindowListOption, CGWindowID, CGWindowImageOption) -> CGImage?

Returns a composite image based on a dynamically generated list of windows.

Deprecated

init?(windowListFromArrayScreenBounds: CGRect, windowArray: CFArray, imageOption: CGWindowImageOption)

Returns a composite image of the specified windows.

Deprecated

### Data Types

typealias CGWindowID

The data type used to store window identifiers.

struct CGWindowListOption

The data type used to specify the options for gathering a list of windows.

struct CGWindowImageOption

The data type to use to specify the type of image to be generated for a window.

enum CGWindowSharingType

The data type used to specify the sharing mode used by a window.

enum CGWindowBackingType

The data type used to specify the backing option for a given window.

### Constants

Window Sharing Constants

Specifies whether and how windows are shared between applications.

Backing Store Types

Specifies how the window device buffers drawing commands.

Window List Option Constants

Specifies which windows in the current user session to include in a generated list.

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

## See Also

### Services

Quartz Display Services

Provides direct access to features in the macOS window server for configuring and controlling display hardware.

Quartz Event Services

Provides features for managing *event taps*—filters for observing and altering the stream of low-level user input events in macOS.

