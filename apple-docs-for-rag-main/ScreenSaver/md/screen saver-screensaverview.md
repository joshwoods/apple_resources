

- Screen Saver
-  ScreenSaverView 

Class

# ScreenSaverView

An abstract class that defines the interface for subclassers to interact with the screen saver infrastructure.

macOS 10.0+

``` source
@MainActor
class ScreenSaverView
```

## Overview

ScreenSaverView provides the interface for your screen saver, including the content you animate onscreen and an optional configuration sheet. Create your own custom subclass and add it to your screen saver bundle. Use your subclass to create the animations that you want to appear onscreen, and to specify additional animation details.

Note

When someone previews your screen saver in System Preferences, the system instantiates your ScreenSaverView subclass.

You can draw from your view’s draw(_:) method, or you can draw directly from the animateOneFrame() method. If you prefer to use the draw(_:) method, use the animateOneFrame() method to call the setNeedsDisplay(_:) method and specify the portions of your view that require updates.

## Topics

### Creating a screen saver view

init?(frame: NSRect, isPreview: Bool)

Creates a newly allocated screen saver view with the specified frame rectangle and preview information.

### Getting the preferred window behavior

class func backingStoreType() -> NSWindow.BackingStoreType

Returns the type of backing store you want for your screen saver’s window.

class func performGammaFade() -> Bool

Indicates whether to perform a gradual screen fade when the system starts and stops your screen saver’s animation.

### Setting and getting the animation time interval

var animationTimeInterval: TimeInterval

The time interval between animation frames.

### Animating the screen saver

func startAnimation()

Activates the periodic timer that animates the screen saver.

func animateOneFrame()

Advances the screen saver’s animation by a single frame.

func stopAnimation()

Deactivates the timer that advances the animation.

var isAnimating: Bool

A Boolean value that indicates whether the screen saver is animating.

### Drawing the view

func draw(NSRect)

Draws the screen saver view.

var isPreview: Bool

A Boolean value that indicates whether the screen saver view is set to a size suitable for previewing its content.

### Accessing the configuration sheet

var hasConfigureSheet: Bool

A Boolean value that indicates whether the screen saver has an associated configuration sheet.

var configureSheet: NSWindow?

The window that contains the controls to configure the screen saver.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

## See Also

### Interface

class ScreenSaverDefaults

A class that defines a set of methods for saving and restoring user defaults for screen savers.

