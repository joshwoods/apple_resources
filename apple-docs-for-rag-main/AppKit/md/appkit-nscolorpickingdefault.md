

- AppKit
-  NSColorPickingDefault 

Protocol

# NSColorPickingDefault

A set of methods that provides basic behavior for a color picker.

macOS

``` source
protocol NSColorPickingDefault
```

## Overview

The NSColorPickingDefault protocol, together with the NSColorPickingCustom protocol (which provides implementation-specific behavior), provides an interface for adding color pickers to an app’s color panel.

## Topics

### Creating Color Pickers

init?(pickerMask: Int, colorPanel: NSColorPanel)

Initializes the receiver with a given color panel and its mode.

**Required**

### Configuring Color Pickers

func setMode(NSColorPanel.Mode)

Specifies the receiver’s mode.

**Required**

func insertNewButtonImage(NSImage, in: NSButtonCell)

Sets the image of a given button cell.

**Required**

func provideNewButtonImage() -> NSImage

Provides the image of the button used to select the receiver in the color panel.

**Required**

func minContentSize() -> NSSize

Indicates the receiver’s minimum content size.

**Required**

func buttonToolTip() -> String

Provides the toolbar button help tag.

**Required**

### Handling Events

func alphaControlAddedOrRemoved(Any?)

Sent when the color panel’s opacity controls have been hidden or displayed.

**Required**

func viewSizeChanged(Any?)

Tells the recever when the color panel’s view size changes in a way that might affect the color picker.

**Required**

### Managing Color Lists

func attachColorList(NSColorList)

Tells the receiver to attach the given color list, if it isn’t already displaying the list.

**Required**

func detachColorList(NSColorList)

Tells the receiver to detach the given color list, unless the receiver isn’t displaying the list.

**Required**

## Relationships

### Inherited By

- NSColorPickingCustom

### Conforming Types

- NSColorPicker

## See Also

### Color Panels

class NSColorPanel

A standard user interface for selecting color in an app.

protocol NSColorPickingCustom

A set of methods that provides a way to add color pickers—custom user interfaces for color selection—to an app’s color panel.

class NSColorPicker

An abstract superclass that implements the default color picking protocol.

