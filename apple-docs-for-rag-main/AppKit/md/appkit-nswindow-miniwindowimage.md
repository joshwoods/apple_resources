

- AppKit
- NSWindow
-  miniwindowImage 

Instance Property

# miniwindowImage

The custom miniaturized window image of the window.

macOS

``` source
@MainActor
var miniwindowImage: NSImage? { get set }
```

## Discussion

The miniaturized window image is the image displayed in the Dock when the window is minimized. If you did not assign a custom image to the window, the value of this property is `nil`.

When the user minimizes the window, the Dock displays miniwindowImage in the corresponding Dock tile, scaling it as needed to fit in the tile. If you do not specify a custom image using this property, the Dock creates one for you automatically.

You can also set this property as needed to change the minimized window image. Typically, you would specify a custom image immediately prior to a window being minimized—when the system posts willMiniaturizeNotification. You can set this property while the window is minimized to update the current image in the Dock. However, you should not use this property to create complex animations in the Dock.

Support for custom images is disabled by default. To enable support, set the `AppleDockIconEnabled` key to true when first registering your application’s user defaults. You must set this key prior to calling the `init` method of NSApplication, which reads the current value of the key.

## See Also

### Minimizing Windows

var isMiniaturized: Bool

A Boolean value that indicates whether the window is minimized.

func performMiniaturize(Any?)

Simulates the user clicking the minimize button by momentarily highlighting the button, then minimizing the window.

func miniaturize(Any?)

Removes the window from the screen list and displays the minimized window in the Dock.

func deminiaturize(Any?)

De-minimizes the window.

var miniwindowTitle: String!

The title displayed in the window’s minimized window.

