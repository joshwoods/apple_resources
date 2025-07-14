

- AppKit
-  NSPanel 

Class

# NSPanel

A special kind of window that typically performs a function that is auxiliary to the main window.

macOS

``` source
@MainActor
class NSPanel
```

## Overview

For details about how panels work (especially to find out how their behavior differs from window behavior), see How Panels Work.

## Topics

### Configuring Panels

var isFloatingPanel: Bool

A Boolean value that indicates whether the receiver is a floating panel.

var becomesKeyOnlyIfNeeded: Bool

A Boolean value that indicates whether the receiver becomes the key window only when needed.

var worksWhenModal: Bool

A Boolean value that indicates whether the panel receives keyboard and mouse events even when some other window is being run modally.

### Constants

Alert Panel Return Values

These constants define values returned by the NSRunAlertPanel function and by the `NSApplication` method runModalSession(_:) when the modal session is run with an `NSPanel` provided by the NSGetAlertPanel function.

Modal Panel Return Values

These constants define the possible return values for such methods as the `runModal...` methods of the NSOpenPanel class, which tell which button (OK or Cancel) the user has clicked on an open panel.

Style Masks

Constants that specify panel styles.

## Relationships

### Inherits From

- NSWindow

### Inherited By

- NSColorPanel
- NSFontPanel
- NSSavePanel

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

### Windows

class NSWindow

A window that an app displays on the screen.

protocol NSWindowDelegate

A set of optional methods that a window’s delegate can implement to respond to events, such as window resizing, moving, exposing, and minimizing.

class NSWindowTab

A tab associated with a window that is part of a tabbing group.

class NSWindowTabGroup

A group of windows that display together as a single tabbed window.

