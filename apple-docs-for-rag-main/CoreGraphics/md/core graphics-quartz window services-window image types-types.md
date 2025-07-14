

- Core Graphics
- Quartz Window Services
-  Window Image Types 

API Collection

# Window Image Types

Specifies the options for capturing an image of a window.

## Topics

### Constants

static var boundsIgnoreFraming: CGWindowImageOption

static var shouldBeOpaque: CGWindowImageOption

static var onlyShadows: CGWindowImageOption

static var bestResolution: CGWindowImageOption

When capturing the window, return the best image resolution. The returned image size may be different than the screen size.

static var nominalResolution: CGWindowImageOption

When capturing the window, return the nominal image resolution. The returned image size is the same as the screen size.

## See Also

### Constants

Window Sharing Constants

Specifies whether and how windows are shared between applications.

Backing Store Types

Specifies how the window device buffers drawing commands.

Window List Option Constants

Specifies which windows in the current user session to include in a generated list.

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

