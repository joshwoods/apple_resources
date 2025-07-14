

- MediaExtension
-  MERAWProcessorExtension 

Protocol

# MERAWProcessorExtension

A protocol that defines a factory to create RAW processors for a codec type that the extension implements.

macOS 15.0+

``` source
protocol MERAWProcessorExtension : NSObjectProtocol
```

## Discussion

This protocol provides a factory method to create a new MERAWProcessor instance for a codecType implemented by the extension. The Video Toolbox instantiates a single MERAWProcessorExtension, and creates individual MERAWProcessor instances as needed. If the `CMVideoFormatDescription` passed to makeProcessor(formatDescription:pixelBufferManager:) is not compatible with the MERAWProcessor implementation, the factory call should fail and return MEError.Code.unsupportedFeature.

## Topics

### Creating an extension

init()

Creates a video RAW processor factory.

**Required**

### Creating a RAW processor

func makeProcessor(formatDescription: CMVideoFormatDescription, pixelBufferManager: MERAWProcessorPixelBufferManager) throws -> any MERAWProcessor

A factory method to create a video RAW processor.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### RAW processors

protocol MERAWProcessor

A protocol that defines the requirements for a RAW processor.

class MERAWProcessorPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

class MERAWProcessingParameter

An object for the RAW processor to describe each processing parameter the processor exposes.

enum MERAWProcessorNotification

Notifications that indicate a RAW processor state change.

RAW processor property list dictionary

Include a property list dictionary to describe a RAW processor.

RAW processor entitlement

Include an entitlement to indicate your extension is a MediaExtension RAW processor.

