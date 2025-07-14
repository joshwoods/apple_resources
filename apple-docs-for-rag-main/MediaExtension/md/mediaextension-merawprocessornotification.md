

- MediaExtension
-  MERAWProcessorNotification 

Enumeration

# MERAWProcessorNotification

Notifications that indicate a RAW processor state change.

macOS 15.0+

``` source
enum MERAWProcessorNotification
```

## Topics

### Type Properties

static let readyForMoreMediaDataDidChange: NSNotification.Name

A notification that indicates a change to the object’s readiness to process additional media data.

static let valuesDidChange: NSNotification.Name

A notification that indicates a change to the object’s set of available processing parameters.

## See Also

### RAW processors

protocol MERAWProcessor

A protocol that defines the requirements for a RAW processor.

protocol MERAWProcessorExtension

A protocol that defines a factory to create RAW processors for a codec type that the extension implements.

class MERAWProcessorPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

class MERAWProcessingParameter

An object for the RAW processor to describe each processing parameter the processor exposes.

RAW processor property list dictionary

Include a property list dictionary to describe a RAW processor.

RAW processor entitlement

Include an entitlement to indicate your extension is a MediaExtension RAW processor.

