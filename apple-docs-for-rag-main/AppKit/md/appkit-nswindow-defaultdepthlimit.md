

- AppKit
- NSWindow
-  defaultDepthLimit 

Type Property

# defaultDepthLimit

Returns the default depth limit for instances of `NSWindow`.

macOS

``` source
@MainActor
class var defaultDepthLimit: NSWindow.Depth { get }
```

## Return Value

The default depth limit for instances of `NSWindow`, determined by the depth of the deepest screen level available to the window server.

## Discussion

The value returned can be examined with the Application Kit functions isPlanar, colorSpaceName, bitsPerSample, and bitsPerPixel.

## See Also

### Related Documentation

func canStoreColor() -> Bool

Indicates whether the window has a depth limit that allows it to store color values.

Deprecated

### Accessing Window Information

var depthLimit: NSWindow.Depth

The depth limit of the window.

var hasDynamicDepthLimit: Bool

A Boolean value that indicates whether the window’s depth limit can change to match the depth of the screen it’s on.

var windowNumber: Int

The window number of the window’s window device.

class func windowNumbers(options: NSWindow.NumberListOptions) -> [NSNumber]?

Returns the window numbers for all visible windows satisfying the specified options.

var deviceDescription: [NSDeviceDescriptionKey : Any]

A dictionary containing information about the window’s resolution, such as color, depth, and so on.

struct NSDeviceDescriptionKey

These constants are the keys for device description dictionaries.

var canBecomeVisibleWithoutLogin: Bool

A Boolean value that indicates whether the window can be displayed at the login window.

var sharingType: NSWindow.SharingType

A Boolean value that indicates the level of access other processes have to the window’s content.

var backingType: NSWindow.BackingStoreType

The window’s backing store type.

func displayLink(target: Any, selector: Selector) -> CADisplayLink

