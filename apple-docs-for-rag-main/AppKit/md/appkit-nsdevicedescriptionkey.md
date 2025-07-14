

- AppKit
-  NSDeviceDescriptionKey 

Structure

# NSDeviceDescriptionKey

These constants are the keys for device description dictionaries.

macOS

``` source
struct NSDeviceDescriptionKey
```

## Topics

### Type Properties

static let bitsPerSample: NSDeviceDescriptionKey

The corresponding value is an `NSNumber` object containing an integer that gives the bit depth of the window’s raster image (2-bit, 8-bit, and so forth).

static let colorSpaceName: NSDeviceDescriptionKey

The corresponding value is an `NSString` object giving the name of the window’s color space.

static let isPrinter: NSDeviceDescriptionKey

If there is a corresponding value, this indicates that the display device is a printer.

static let isScreen: NSDeviceDescriptionKey

If there is a corresponding value, this indicates that the display device is a screen.

static let resolution: NSDeviceDescriptionKey

The corresponding value is an `NSValue` object containing a value of type `NSSize` that describes the window’s raster resolution in dots per inch (dpi).

static let size: NSDeviceDescriptionKey

The corresponding value is an `NSValue` object containing a value of type `NSSize` that gives the size of the window’s frame rectangle.

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var colorSpace: NSColorSpace?

The color space of the screen.

var localizedName: String

The localized name of the display.

func canRepresent(NSDisplayGamut) -> Bool

A Boolean value indicating whether the color space of the screen is capable of representing the specified display gamut.

enum NSDisplayGamut

class var screensHaveSeparateSpaces: Bool

Returns a Boolean value indicating whether each screen can have its own set of spaces.

