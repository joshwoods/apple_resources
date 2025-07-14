

- Quartz
- Quartz Composer
-  QCCompositionPickerViewDelegate 

# QCCompositionPickerViewDelegate

The `QCCompositionPickerViewDelegate` informal protocol defines methods that allow your application to respond to changes in a composition picker view (a QCCompositionPickerView object).

## Topics

### Responding to Composition Selections

func compositionPickerView(_ pickerView: QCCompositionPickerView!, didSelect composition: QCComposition!)

Performs custom tasks when the selected composition in the composition picker view changes.

Deprecated

### Responding to Animation State Changes

func compositionPickerViewDidStartAnimating(_ pickerView: QCCompositionPickerView!)

Performs custom tasks when the composition picker view starts animating a composition.

Deprecated

func compositionPickerViewWillStopAnimating(_ pickerView: QCCompositionPickerView!)

Performs custom tasks when the composition picker view stops animating a composition.

Deprecated

## See Also

### Protocols

QCCompositionParameterViewDelegate

A protocol for composition parameter view’s delegate.

protocol QCCompositionRenderer

The `QCRenderer` protocol defines the methods used to pass data to the input ports or retrieve data from the output ports of the root patch of a Quartz Composer composition. This protocol is adopted by the QCRenderer, QCView, and QCCompositionLayer classes.

Deprecated

protocol QCPlugInContext

The `QCPlugInContext` protocol defines methods that you use only from within the execution method (execute(_:atTime:withArguments:)) of a `QCPlugIn` object.

Deprecated

protocol QCPlugInInputImageSource

The `QCPlugInInputImageSource` protocol eliminates the need to use explicit image types for the image input ports on your custom patch. Not only does using the protocol avoid restrictions of a specific image type, but it avoids impedance mismatches, and provides better performance by deferring pixel computation until it is needed. When you need to access the pixels in an image, you simply convert the image to a representation (texture or buffer) using one of the methods defined by the `QCPlugInInputImageSource` protocol. Use a texture representation when you want to use input images on the GPU. Use a buffer representation when you want to use input images on the CPU.

Deprecated

protocol QCPlugInOutputImageProvider

The `QCPlugInOuputImageProvider` protocol eliminates the need to use explicit image types for the image output ports on a custom patch. The methods in this protocol are called by the Quartz Composer engine when the output image is needed. If your custom patch has an image output port, you need to implement the appropriate methods for rendering image data and to supply information about the rendering destination and the image bounds.

Deprecated

