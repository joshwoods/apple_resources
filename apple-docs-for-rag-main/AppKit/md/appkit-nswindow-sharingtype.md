

- AppKit
- NSWindow
-  sharingType 

Instance Property

# sharingType

A Boolean value that indicates the level of access other processes have to the window’s content.

macOS 10.5+

``` source
@MainActor
var sharingType: NSWindow.SharingType { get set }
```

## Discussion

The value of this property represents the sharing level of the window’s content. See NSWindow.SharingType for possible values.

## See Also

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

var deviceDescription: [NSDeviceDescriptionKey : Any]

A dictionary containing information about the window’s resolution, such as color, depth, and so on.

struct NSDeviceDescriptionKey

These constants are the keys for device description dictionaries.

var canBecomeVisibleWithoutLogin: Bool

A Boolean value that indicates whether the window can be displayed at the login window.

var backingType: NSWindow.BackingStoreType

The window’s backing store type.

func displayLink(target: Any, selector: Selector) -> CADisplayLink

