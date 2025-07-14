

- Quartz
-  Quartz Composer Deprecated

API Collection

# Quartz Composer

macOS 10.4–10.15Deprecated

## Topics

### Classes

class QCComposition

The `QCComposition` class represents a Quartz Composer composition that either:

class QCCompositionLayer

A layer that loads, plays, and controls Quartz Composer compositions in a Core Animation layer hierarchy.

class QCCompositionParameterView

A class that allows users to edit the input parameters of a composition in real time. The composition can be rendering in any of the following objects: QCRenderer, QCView, or QCCompositionLayer.

class QCCompositionPickerPanel

The `QCCompositionPickerPanel` class represents a utility window that allows users to browse compositions that are in the Quartz Composer composition repository and, if supported, preview the composition. The `QCCompositionPickerPanel` class cannot be subclassed.

class QCCompositionPickerView

The `QCCompositionPickerView` class allows users to browse compositions that are in the Quartz Composer composition repository, and to preview them. You can set the default input parameters for a composition preview by using the method setDefaultValue:forInputKey:.

class QCCompositionRepository

The `QCCompositionRepository` class represents a system-wide centralized repository of built-in and installed Quartz Composer compositions (`/Library/Compositions` and `~/Library/Compositions`). The `QCCompositionRepository` class cannot be subclassed.

class QCPatchController

class QCPlugIn

A base class to subclass for writing custom patches.

class QCPlugInViewController

The `QCPlugInViewController` class communicates (through Cocoa bindings) between a custom patch and the view used for the internal settings of the custom patch. Only custom patches that use internal settings exposed to the user need to use the `QCPlugInViewController` class.

class QCRenderer

A base class for low-level rendering.

class QCView

The `QCView` class is a custom `NSView` class that loads, plays, and controls Quartz Composer compositions. It is an autonomous view that is driven by an internal timer running on the main thread.

### Protocols

QCCompositionParameterViewDelegate

A protocol for composition parameter view’s delegate.

QCCompositionPickerViewDelegate

The `QCCompositionPickerViewDelegate` informal protocol defines methods that allow your application to respond to changes in a composition picker view (a QCCompositionPickerView object).

protocol QCCompositionRenderer

The `QCRenderer` protocol defines the methods used to pass data to the input ports or retrieve data from the output ports of the root patch of a Quartz Composer composition. This protocol is adopted by the QCRenderer, QCView, and QCCompositionLayer classes.

protocol QCPlugInContext

The `QCPlugInContext` protocol defines methods that you use only from within the execution method (execute(_:atTime:withArguments:)) of a `QCPlugIn` object.

protocol QCPlugInInputImageSource

The `QCPlugInInputImageSource` protocol eliminates the need to use explicit image types for the image input ports on your custom patch. Not only does using the protocol avoid restrictions of a specific image type, but it avoids impedance mismatches, and provides better performance by deferring pixel computation until it is needed. When you need to access the pixels in an image, you simply convert the image to a representation (texture or buffer) using one of the methods defined by the `QCPlugInInputImageSource` protocol. Use a texture representation when you want to use input images on the GPU. Use a buffer representation when you want to use input images on the CPU.

protocol QCPlugInOutputImageProvider

The `QCPlugInOuputImageProvider` protocol eliminates the need to use explicit image types for the image output ports on a custom patch. The methods in this protocol are called by the Quartz Composer engine when the output image is needed. If your custom patch has an image output port, you need to implement the appropriate methods for rendering image data and to supply information about the rendering destination and the image bounds.

### Structures

struct QCPlugInExecutionMode

Execution modes for custom patches.

struct QCPlugInTimeMode

Time modes for custom patches.

### Reference

Quartz Data Types

Quartz Constants

Quartz Enumerations

Quartz Composer Constants

Quartz Composer Enumerations

