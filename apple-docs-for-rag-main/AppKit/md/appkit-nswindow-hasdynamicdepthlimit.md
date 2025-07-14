

- AppKit
- NSWindow
-  hasDynamicDepthLimit 

Instance Property

# hasDynamicDepthLimit

A Boolean value that indicates whether the window’s depth limit can change to match the depth of the screen it’s on.

macOS

``` source
@MainActor
var hasDynamicDepthLimit: Bool { get }
```

## Discussion

The value of this property is true when the window has a dynamic depth limit; otherwise, false. When the value of hasDynamicDepthLimit is false, the window uses either its preset depth limit or the default depth limit. A different, and non-dynamic, depth limit can be set using the depthLimit property.

## See Also

### Accessing Window Information

var depthLimit: NSWindow.Depth

The depth limit of the window.

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

