

- Quartz
-  QCCompositionRenderer Deprecated

Protocol

# QCCompositionRenderer

The `QCRenderer` protocol defines the methods used to pass data to the input ports or retrieve data from the output ports of the root patch of a Quartz Composer composition. This protocol is adopted by the QCRenderer, QCView, and QCCompositionLayer classes.

macOS 10.4–10.15Deprecated

``` source
protocol QCCompositionRenderer
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Topics

### Passing and Retrieving Values From a Composition

func setValue(Any!, forInputKey: String!) -> Bool

Sets the value for an input port of a composition.

**Required**

func value(forInputKey: String!) -> Any!

Returns the value for an input port of a composition.

**Required**

func value(forOutputKey: String!) -> Any!

Returns the value for an output port of a composition.

**Required**

func value(forOutputKey: String!, ofType: String!) -> Any!

Returns the current value on an output port (identified by its key) of the root patch of the composition.

**Required**

### Getting Input and Output Keys

func inputKeys() -> [Any]!

Returns an array that contains the keys that identify the input ports of the root patch of the composition.

**Required**

func outputKeys() -> [Any]!

Returns an array that contains the keys that identify the output ports of the root patch of the composition.

**Required**

### Getting Attributes

func attributes() -> [AnyHashable : Any]!

Returns the attributes of the composition associated with the renderer.

**Required**

### Storing Arbitrary Information

func userInfo() -> NSMutableDictionary!

Returns a mutable dictionary for storing arbitrary information.

**Required**

### Saving and Restoring Input Values

func propertyListFromInputValues() -> Any!

Returns a property list object that represents the current values for all the input keys of the composition.

**Required**

func setInputValuesWithPropertyList(Any!)

Sets the values for the input keys of the composition from a previously saved property list.

**Required**

## Relationships

### Conforming Types

- QCCompositionLayer
- QCRenderer
- QCView

## See Also

### Protocols

QCCompositionParameterViewDelegate

A protocol for composition parameter view’s delegate.

QCCompositionPickerViewDelegate

The `QCCompositionPickerViewDelegate` informal protocol defines methods that allow your application to respond to changes in a composition picker view (a QCCompositionPickerView object).

protocol QCPlugInContext

The `QCPlugInContext` protocol defines methods that you use only from within the execution method (execute(_:atTime:withArguments:)) of a `QCPlugIn` object.

Deprecated

protocol QCPlugInInputImageSource

The `QCPlugInInputImageSource` protocol eliminates the need to use explicit image types for the image input ports on your custom patch. Not only does using the protocol avoid restrictions of a specific image type, but it avoids impedance mismatches, and provides better performance by deferring pixel computation until it is needed. When you need to access the pixels in an image, you simply convert the image to a representation (texture or buffer) using one of the methods defined by the `QCPlugInInputImageSource` protocol. Use a texture representation when you want to use input images on the GPU. Use a buffer representation when you want to use input images on the CPU.

Deprecated

protocol QCPlugInOutputImageProvider

The `QCPlugInOuputImageProvider` protocol eliminates the need to use explicit image types for the image output ports on a custom patch. The methods in this protocol are called by the Quartz Composer engine when the output image is needed. If your custom patch has an image output port, you need to implement the appropriate methods for rendering image data and to supply information about the rendering destination and the image bounds.

Deprecated

