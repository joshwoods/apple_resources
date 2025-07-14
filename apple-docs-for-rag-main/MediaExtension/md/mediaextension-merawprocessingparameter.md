

- MediaExtension
-  MERAWProcessingParameter 

Class

# MERAWProcessingParameter

An object for the RAW processor to describe each processing parameter the processor exposes.

macOS 15.0+

``` source
class MERAWProcessingParameter
```

## Discussion

This protocol provides an interface for Video Toolbox to query descriptions of the different parameters that can be used to influence RAW processor operation. A distinct MERAWProcessingParameter is created for each parameter supported by the RAW processor, and the set of supported parameters is returned by the processingParameters interface.

## Topics

### Inspecting a processing parameter

var enabled: Bool

A Boolean value that indicates whether the extension enables the parameter.

var key: String

A unique key string identifying the parameter.

var longDescription: String

A localized description of the parameter, suitable for displaying in a tool tip or similar explanatory UI.

var name: String

A localized human-readable name for the parameter, suitable for displaying in application UI.

### Processing parameters

class Boolean

An object that describes a Boolean parameter of a RAW processor.

class FloatingPoint

An object that describes a floating-point parameter of a RAW processor.

class Integer

An object that describes an integer parameter of a RAW processor.

class List

An object that describes a list parameter of a RAW processor.

class ListElement

An object that describes a list element parameter of a RAW processor.

class SubGroup

An object that describes a sub group parameter of a RAW processor.

### Class methods

class func boolean(name: String, key: String, description: String, initialValue: Bool, neutralValue: Bool?, cameraValue: Bool?) -> MERAWProcessingParameter.Boolean

class func integer(name: String, key: String, description: String, initialValue: Int, maximum: Int, minimum: Int, neutralValue: Int?, cameraValue: Int?) -> MERAWProcessingParameter.Integer

class func list(name: String, key: String, description: String, list: [MERAWProcessingParameter.ListElement], initialValue: Int, neutralValue: Int?, cameraValue: Int?) -> MERAWProcessingParameter.List

class func listElement(name: String, description: String, elementID: Int) -> MERAWProcessingParameter.ListElement

class func subGroup(name: String, description: String, parameters: [MERAWProcessingParameter]) -> MERAWProcessingParameter.SubGroup

class func float(name: String, key: String, description: String, initialValue: Float, maximum: Float, minimum: Float, neutralValue: Float?, cameraValue: Float?) -> MERAWProcessingParameter.FloatingPoint

## Relationships

### Inherits From

- NSObject

### Inherited By

- MERAWProcessingParameter.Boolean
- MERAWProcessingParameter.FloatingPoint
- MERAWProcessingParameter.Integer
- MERAWProcessingParameter.List
- MERAWProcessingParameter.ListElement
- MERAWProcessingParameter.SubGroup

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### RAW processors

protocol MERAWProcessor

A protocol that defines the requirements for a RAW processor.

protocol MERAWProcessorExtension

A protocol that defines a factory to create RAW processors for a codec type that the extension implements.

class MERAWProcessorPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

enum MERAWProcessorNotification

Notifications that indicate a RAW processor state change.

RAW processor property list dictionary

Include a property list dictionary to describe a RAW processor.

RAW processor entitlement

Include an entitlement to indicate your extension is a MediaExtension RAW processor.

