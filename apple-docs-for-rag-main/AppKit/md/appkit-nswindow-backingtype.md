

- AppKit
- NSWindow
-  backingType 

Instance Property

# backingType

The window’s backing store type.

macOS

``` source
@MainActor
var backingType: NSWindow.BackingStoreType { get set }
```

## Discussion

The possible values for this property are described in NSWindow.BackingStoreType. You can set the property only to switch a buffered window to retained or vice versa; you can’t change the backing type to or from nonretained after initializing a `NSWindow` object (an error is generated if you attempt to do so).

## See Also

### Related Documentation

convenience init(contentRect: NSRect, styleMask: NSWindow.StyleMask, backing: NSWindow.BackingStoreType, defer: Bool, screen: NSScreen?)

Initializes an allocated window with the specified values.

init(contentRect: NSRect, styleMask: NSWindow.StyleMask, backing: NSWindow.BackingStoreType, defer: Bool)

Initializes the window with the specified values.

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

var sharingType: NSWindow.SharingType

A Boolean value that indicates the level of access other processes have to the window’s content.

func displayLink(target: Any, selector: Selector) -> CADisplayLink

