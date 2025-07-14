

- Quartz
-  QCComposition Deprecated

Class

# QCComposition

The `QCComposition` class represents a Quartz Composer composition that either:

macOS 10.4–10.15Deprecated

``` source
class QCComposition
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Overview

- comes from the system-wide composition repository (`/Library/Compositions` and `~/Library/Compositions`) where it can be accessed by any application through the methods of the QCCompositionRepository class

- is created from an arbitrary source (typically a file on disk) using one of its methods

This class cannot be subclassed.

A `QCComposition` object has the following information associated with it and that you can obtain by using the appropriate method of the `QCComposition` class:

- Attributes include the name and description of the composition, copyright information, and whether or not its provided by macOS (built-in).

- The protocols that the composition conforms to. A *composition protocol* defines a set of required and optional input parameters and output results.

Many methods of the QCRenderer, QCCompositionLayer, and QCView classes take a `QCComposition` object as a parameter.

## Topics

### Creating a Composition

init!(file: String!)

Returns a composition object initialized with a Quartz Composer composition file.

init!(data: Data!)

Returns a composition object initialized with the contents of a Quartz Composer composition file.

### Getting Information About a Composition

func attributes() -> [AnyHashable : Any]!

Returns the attributes of the composition.

func protocols() -> [Any]!

Returns the list of protocols to which the composition conforms.

func identifier() -> String!

Returns the unique and persistent identifier for the composition from the composition repository.

### Getting Port Keys

func inputKeys() -> [Any]!

Returns an array listing the keys that identify the input ports of the root patch of the composition.

func outputKeys() -> [Any]!

Returns an array listing the keys that identify the output ports of the root patch of the composition.

### Constants

Attribute Keys

Attributes of a composition.

Composition Categories

Categories for compositions.

Standard Protocol Input Keys

Input ports of a composition.

Standard Protocol Output Keys

Output ports of a composition.

Standard Protocols

Protocols for a composition.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Classes

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

class QCPlugInViewController

The `QCPlugInViewController` class communicates (through Cocoa bindings) between a custom patch and the view used for the internal settings of the custom patch. Only custom patches that use internal settings exposed to the user need to use the `QCPlugInViewController` class.

Deprecated

class QCRenderer

A base class for low-level rendering.

Deprecated

class QCView

The `QCView` class is a custom `NSView` class that loads, plays, and controls Quartz Composer compositions. It is an autonomous view that is driven by an internal timer running on the main thread.

Deprecated

