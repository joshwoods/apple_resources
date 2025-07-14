

- AppKit
- NSScreen
-  canRepresent(\_:) 

Instance Method

# canRepresent(\_:)

A Boolean value indicating whether the color space of the screen is capable of representing the specified display gamut.

macOS 10.12+

``` source
func canRepresent(_ displayGamut: NSDisplayGamut) -> Bool
```

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

enum NSDisplayGamut

class var screensHaveSeparateSpaces: Bool

Returns a Boolean value indicating whether each screen can have its own set of spaces.

