

- AppKit
- NSWindow
-  depthLimit 

Instance Property

# depthLimit

The depth limit of the window.

macOS

``` source
@MainActor
var depthLimit: NSWindow.Depth { get set }
```

## Discussion

The value of this property can be examined with the Application Kit functions isPlanar, colorSpaceName, bitsPerSample, and bitsPerPixel. In addition, the NSBestDepth function provides the best depth limit based on a set of parameters.

Setting this property to `0` sets the depth limit to the window’s default depth limit. A depth limit of `0` can be useful for reverting a window object to its initial depth. You can also use one of the explicit bit depths defined in `Explicit Window Depth Limits` (NSWindow.Depth.twentyfourBitRGB is the default).

## See Also

### Accessing Window Information

var hasDynamicDepthLimit: Bool

A Boolean value that indicates whether the window’s depth limit can change to match the depth of the screen it’s on.

class var defaultDepthLimit: NSWindow.Depth

Returns the default depth limit for instances of `NSWindow`.

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

