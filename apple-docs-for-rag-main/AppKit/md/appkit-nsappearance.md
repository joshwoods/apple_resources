

- AppKit
-  NSAppearance 

Class

# NSAppearance

An object that manages standard appearance attributes for UI elements in an app.

macOS 10.9+

``` source
class NSAppearance
```

## Mentioned in 

Choosing a Specific Appearance for Your macOS App

## Overview

An NSAppearance object manages how AppKit renders your app’s UI elements. Specifically, appearance objects determine which colors and images AppKit uses when drawing windows, views, and controls. Although you can use an appearance object to determine how to draw custom views and controls, a better approach is to choose colors and images that adapt automatically to the current appearance. For example, define a color asset whose actual color value changes for light and dark appearances. You can assign specific appearances to your views in Interface Builder.

The user chooses the default appearance for the system, but you can override that appearance for all or part of your app. Apps inherit the default system appearance, windows inherit their app’s appearance, and views inherit the appearance of their nearest ancestor (either a superview or window). To force a window or view to adopt an appearance, assign a specific appearance object to its appearance property.

When AppKit draws a control, it automatically sets the current appearance on the current thread to the control’s appearance. The current appearance influences the drawing path and return values you get when you access system fonts and colors. The current appearance also affects the appearance of text and images, such as the text and template images in a toolbar.

## Topics

### Creating an Appearance

init?(named: NSAppearance.Name)

Creates an appearance object based on the name of one of the standard system appearances.

init?(appearanceNamed: NSAppearance.Name, bundle: Bundle?)

Creates an appearance object from the named appearance file located in the specified bundle.

init?(coder: NSCoder)

### Getting the Appearance Name

var name: NSAppearance.Name

The name of the appearance.

struct Name

### Determining the Most Appropriate Appearance

func bestMatch(from: [NSAppearance.Name]) -> NSAppearance.Name?

Returns the appearance name that most closely matches the current appearance object.

### Getting and Setting the Current Appearance

class func currentDrawing() -> NSAppearance

The appearance that the system uses for color and asset resolution, and that’s active for drawing, usually from locking focus on a view.

func performAsCurrentDrawingAppearance(() -> Void)

Sets the appearance to be the active drawing appearance and perform the specified block.

class var current: NSAppearance!

Returns the appearance object that’s active on the current thread.

Deprecated

### Managing Vibrancy

var allowsVibrancy: Bool

Specifies whether the current appearance allows vibrancy.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Appearance System

protocol NSAppearanceCustomization

A set of methods for getting and setting the appearance attributes of a view.

