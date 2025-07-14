

- AppKit
- NSWindow
-  windowNumbers(options:) 

Type Method

# windowNumbers(options:)

Returns the window numbers for all visible windows satisfying the specified options.

macOS 10.6+

``` source
@MainActor
class func windowNumbers(options: NSWindow.NumberListOptions = []) -> [NSNumber]?
```

## Parameters 

`options`  

The possible options are specified in NSWindow.NumberListOptions.

## Return Value

An array of window numbers for all visible windows satisfying the specified options. (Windows on the active space are returned in z-order; that is, front to back.)

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

