

- AppKit
- NSScreen
-  deviceDescription 

Instance Property

# deviceDescription

The device dictionary for the screen.

macOS

``` source
var deviceDescription: [NSDeviceDescriptionKey : Any] { get }
```

## Discussion

This is a dictionary containing the attributes of the receiver’s screen. For the list of keys you can use to retrieve values from the returned dictionary, see `Display Device—Descriptions`.

In addition to the display device constants described in NSWindow, you can also retrieve the CGDirectDisplayID value associated with the screen from this dictionary. To access this value, specify the Objective-C string `@"NSScreenNumber"` as the key when requesting the item from the dictionary. The value associated with this key is an NSNumber object containing the display ID value. This string is only valid when used as a key for the dictionary returned by this method.

## See Also

### Getting Screen Information

var depth: NSWindow.Depth

The current bit depth and colorspace information of the screen.

var frame: NSRect

The dimensions and location of the screen.

var supportedWindowDepths: UnsafePointer&lt;NSWindow.Depth>

A zero-terminated array of the window depths supported by the screen.

struct NSDeviceDescriptionKey

These constants are the keys for device description dictionaries.

var colorSpace: NSColorSpace?

The color space of the screen.

var localizedName: String

The localized name of the display.

func canRepresent(NSDisplayGamut) -> Bool

A Boolean value indicating whether the color space of the screen is capable of representing the specified display gamut.

enum NSDisplayGamut

class var screensHaveSeparateSpaces: Bool

Returns a Boolean value indicating whether each screen can have its own set of spaces.

