

- AppKit
-  NSFontPanel 

Class

# NSFontPanel

The Font panel—a user interface object that displays a list of available fonts, letting the user preview them and change the font used to display text.

macOS

``` source
@MainActor
class NSFontPanel
```

## Overview

Actual changes to the font panel are made through conversion messages sent to the shared NSFontManager instance. There’s only one Font panel for each app.

## Topics

### Getting the Font Panel

class var shared: NSFontPanel

Returns the single `NSFontPanel` instance for the application, creating it if necessary.

class var sharedFontPanelExists: Bool

Returns true if the shared Font panel has been created, false if it hasn’t.

### Enabling Font Changes

var isEnabled: Bool

A Boolean that shows whether the receiver’s Set button is enabled.

func reloadDefaultFontFamilies()

Triggers a reload to the default state, so that the delegate is called.

### Updating the Font Panel

func setPanelFont(NSFont, isMultiple: Bool)

Sets the selected font in the receiver to the specified font.

### Converting Fonts

func convert(NSFont) -> NSFont

Converts the specified font using the settings in the receiver, with the aid of the shared `NSFontManager` if necessary.

### Working in Modal Loops

var worksWhenModal: Bool

A Boolean that indicates whether the receiver allows fonts to be changed in modal windows and panels.

### Setting an Accessory View

var accessoryView: NSView?

The specified view as the receiver’s accessory view, allowing you to add custom controls to your application’s Font panel without having to create a subclass.

### Structures

struct ModeMask

## Relationships

### Inherits From

- NSPanel

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
- NSMenuItemValidation
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- Sendable

## See Also

### Font Panels

struct ModeMask

NSFontPanelValidation

A set of methods you use to tell the Font panel to display some or all of its elements.

protocol NSFontChanging

