

- AppKit
- NSView
-  isInFullScreenMode 

Instance Property

# isInFullScreenMode

A Boolean value indicating whether the view is in full screen mode.

macOS 10.5+

``` source
@MainActor
var isInFullScreenMode: Bool { get }
```

## Discussion

The value of this property is true when the view is in full screen mode or false when it is not.

## See Also

### Drawing the View in Fullscreen Mode

func enterFullScreenMode(NSScreen, withOptions: [NSView.FullScreenModeOptionKey : Any]?) -> Bool

Sets the view to full screen mode.

func exitFullScreenMode(options: [NSView.FullScreenModeOptionKey : Any]?)

Instructs the view to exit full screen mode.

struct FullScreenModeOptionKey

These constants are keys that you can use in the options dictionary in enterFullScreenMode(_:withOptions:) and exitFullScreenMode(options:).

