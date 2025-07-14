

- Quartz
-  QCPlugInViewController Deprecated

Class

# QCPlugInViewController

The `QCPlugInViewController` class communicates (through Cocoa bindings) between a custom patch and the view used for the internal settings of the custom patch. Only custom patches that use internal settings exposed to the user need to use the `QCPlugInViewController` class.

macOS 10.4–10.15Deprecated

``` source
@MainActor
class QCPlugInViewController
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Overview

You access the internal settings of a custom patch through key-value coding (KVC). All the KVC keys that represent the internal settings of the custom patch must be listed in its `plugInKeys` method.

The view controller for a custom patch expects

- the nib file `File's Owner` class set to the `QCPlugInViewController` class

- the view outlet connected to the view that contains the editing controls

The controls are bound to the `File's Owner` as the target and `plugIn.XXX` as the model key path, where `XXX` is the KVC key for a given internal setting of the custom patch instance.

## Topics

### Creating a Controller

init!(plugIn: QCPlugIn!, viewNibName: String!)

Creates and initializes a controller for the specified `QCPlugIn` object and nib file.

### Getting the QCPlugIn Object

func plugIn() -> QCPlugIn!

Returns the `QCPlugIn` object associated with the view controller for the custom patch.

## Relationships

### Inherits From

- NSViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Related Documentation

Quartz Composer Custom Patch Programming Guide

### Classes

class QCComposition

The `QCComposition` class represents a Quartz Composer composition that either:

Deprecated

class QCCompositionLayer

A layer that loads, plays, and controls Quartz Composer compositions in a Core Animation layer hierarchy.

Deprecated

class QCCompositionParameterView

A class that allows users to edit the input parameters of a composition in real time. The composition can be rendering in any of the following objects: QCRenderer, QCView, or QCCompositionLayer.

Deprecated

class QCCompositionPickerPanel

The `QCCompositionPickerPanel` class represents a utility window that allows users to browse compositions that are in the Quartz Composer composition repository and, if supported, preview the composition. The `QCCompositionPickerPanel` class cannot be subclassed.

Deprecated

class QCCompositionPickerView

The `QCCompositionPickerView` class allows users to browse compositions that are in the Quartz Composer composition repository, and to preview them. You can set the default input parameters for a composition preview by using the method setDefaultValue:forInputKey:.

Deprecated

class QCCompositionRepository

The `QCCompositionRepository` class represents a system-wide centralized repository of built-in and installed Quartz Composer compositions (`/Library/Compositions` and `~/Library/Compositions`). The `QCCompositionRepository` class cannot be subclassed.

Deprecated

class QCPatchControllerDeprecated

class QCPlugIn

A base class to subclass for writing custom patches.

Deprecated

class QCRenderer

A base class for low-level rendering.

Deprecated

class QCView

The `QCView` class is a custom `NSView` class that loads, plays, and controls Quartz Composer compositions. It is an autonomous view that is driven by an internal timer running on the main thread.

Deprecated

