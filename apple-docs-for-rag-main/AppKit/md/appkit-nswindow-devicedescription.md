

- AppKit
- NSWindow
-  deviceDescription 

Instance Property

# deviceDescription

A dictionary containing information about the window’s resolution, such as color, depth, and so on.

macOS

``` source
@MainActor
var deviceDescription: [NSDeviceDescriptionKey : Any] { get }
```

## Discussion

This information is useful for tuning images and colors to the window’s display capabilities. The contents of the dictionary are described in `Display Device—Descriptions`.

## See Also

### Related Documentation

func usingColorSpaceName(NSColorSpaceName) -> NSColor?

Creates a new color object whose color is the same as the receiver’s, except that the new color object is in the specified color space.

Deprecated

var deviceDescription: [NSDeviceDescriptionKey : Any]

The device dictionary for the screen.

### Accessing Window Information

var depthLimit: NSWindow.Depth

The depth limit of the window.

var hasDynamicDepthLimit: Bool

A Boolean value that indicates whether the window’s depth limit can change to match the depth of the screen it’s on.

class var defaultDepthLimit: NSWindow.Depth

Returns the default depth limit for instances of `NSWindow`.

var windowNumber: Int

The window number of the window’s window device.

class func windowNumbers(options: NSWindow.NumberListOptions) -> [NSNumber]?

Returns the window numbers for all visible windows satisfying the specified options.

struct NSDeviceDescriptionKey

These constants are the keys for device description dictionaries.

var canBecomeVisibleWithoutLogin: Bool

A Boolean value that indicates whether the window can be displayed at the login window.

var sharingType: NSWindow.SharingType

A Boolean value that indicates the level of access other processes have to the window’s content.

var backingType: NSWindow.BackingStoreType

The window’s backing store type.

func displayLink(target: Any, selector: Selector) -> CADisplayLink

