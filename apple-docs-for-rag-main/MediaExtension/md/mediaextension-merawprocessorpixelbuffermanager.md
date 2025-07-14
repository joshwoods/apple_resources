

- MediaExtension
-  MERAWProcessorPixelBufferManager 

Class

# MERAWProcessorPixelBufferManager

Describes pixel buffer requirements and creates new pixel buffers.

macOS 15.0+

``` source
class MERAWProcessorPixelBufferManager
```

## Discussion

It contains the interfaces that the MERAWProcessor uses for two tasks. First, to declare its set of requirements for output CVPixelBuffer in the form of a pixelBufferAttributes dictionary. Second, create pixel buffers that match processor output requirements and satisfy Video Toolbox and client requirements.

## Topics

### Creating a pixel buffer

var pixelBufferAttributes: [String : any Sendable]

A dictionary that contains the attributes Video Toolbox uses to create a pixel buffer for the video RAW processor.

func makePixelBuffer() throws -> CVPixelBuffer

Generates a pixel buffer using the session’s pixel buffer pool.

## Relationships

### Inherits From

- NSObject

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

class MERAWProcessingParameter

An object for the RAW processor to describe each processing parameter the processor exposes.

enum MERAWProcessorNotification

Notifications that indicate a RAW processor state change.

RAW processor property list dictionary

Include a property list dictionary to describe a RAW processor.

RAW processor entitlement

Include an entitlement to indicate your extension is a MediaExtension RAW processor.

