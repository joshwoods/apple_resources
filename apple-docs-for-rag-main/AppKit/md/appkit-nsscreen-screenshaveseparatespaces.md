

- AppKit
- NSScreen
-  screensHaveSeparateSpaces 

Type Property

# screensHaveSeparateSpaces

Returns a Boolean value indicating whether each screen can have its own set of spaces.

macOS 10.9+

``` source
class var screensHaveSeparateSpaces: Bool { get }
```

## Discussion

This method reflects whether the “Displays have separate Spaces” option is enabled in Mission Control system preference. You might use the return value to determine how to present your app when in fullscreen mode.

## See Also

### Getting Screen Information

var depth: NSWindow.Depth

The current bit depth and colorspace information of the screen.

var frame: NSRect

The dimensions and location of the screen.

var supportedWindowDepths: UnsafePointer&lt;NSWindow.Depth>

A zero-terminated array of the window depths supported by the screen.

var deviceDescription: [NSDeviceDescriptionKey : Any]

The device dictionary for the screen.

struct NSDeviceDescriptionKey

These constants are the keys for device description dictionaries.

var colorSpace: NSColorSpace?

The color space of the screen.

var localizedName: String

The localized name of the display.

func canRepresent(NSDisplayGamut) -> Bool

A Boolean value indicating whether the color space of the screen is capable of representing the specified display gamut.

enum NSDisplayGamut

