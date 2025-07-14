

- Quartz
-  QCCompositionLayer Deprecated

Class

# QCCompositionLayer

A layer that loads, plays, and controls Quartz Composer compositions in a Core Animation layer hierarchy.

macOS 10.5–10.14Deprecated

``` source
class QCCompositionLayer
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Overview

The composition tracks the Core Animation layer time and is rendered directly at the current dimensions of the QCCompositionLayer object.

An archived `QCCompositionLayer` object saves the composition that’s loaded at the time the layer is archived. It detects layer usage and pauses or resumes the composition appropriately. A `QCCompositionLayer` object starts rendering the composition automatically when the layer is placed in a visible layer hierarchy. The layer stops rendering when it is hidden or removed from the visible layer hierarchy.

You can pass data to the input ports, or retrieve data from the output ports, of the root patch of a composition by accessing the `patch` attribute of the `QCCompositionLayer` instance using methods provided by the QCCompositionRenderer protocol.

Note

You must not modify the `asynchronous` property of the superclass CAOpenGLLayer.

## Topics

### Creating a Composition Layer

init!(file: String!)

Initializes and returns a composition layer using the Quartz Composer composition in the specified file.

init!(composition: QCComposition!)

Initializes and returns a composition layer using the provided Quartz Composer composition.

### Getting the Composition

func composition() -> QCComposition!

Returns the composition associated with the layer.

## Relationships

### Inherits From

- CAOpenGLLayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- QCCompositionRenderer

## See Also

### Classes

class QCComposition

The `QCComposition` class represents a Quartz Composer composition that either:

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

