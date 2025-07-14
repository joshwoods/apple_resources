

- AppKit
- NSWindow
-  windowNumber 

Instance Property

# windowNumber

The window number of the window’s window device.

macOS

``` source
@MainActor
var windowNumber: Int { get }
```

## Discussion

Each window device in an application is given a unique window number—note that this isn’t the same as the global window number assigned by the window server. This number can be used to identify the window device with the order(_:relativeTo:) method and in the AppKit function NSWindowList.

If the window doesn’t have a window device, the value of this property is equal to or less than `0`.

## See Also

### Related Documentation

var isOneShot: Bool

A Boolean value that indicates whether the window device the window manages is freed when it’s removed from the screen list.

Deprecated

init(contentRect: NSRect, styleMask: NSWindow.StyleMask, backing: NSWindow.BackingStoreType, defer: Bool)

Initializes the window with the specified values.

### Accessing Window Information

var depthLimit: NSWindow.Depth

The depth limit of the window.

var hasDynamicDepthLimit: Bool

A Boolean value that indicates whether the window’s depth limit can change to match the depth of the screen it’s on.

class var defaultDepthLimit: NSWindow.Depth

Returns the default depth limit for instances of `NSWindow`.

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

