

- Create ML Components
-  AudioConvertingTransformer 

Structure

# AudioConvertingTransformer

A transformer for audio conversion.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct AudioConvertingTransformer
```

## Topics

### Creating the transformer

init(targetFormat: AVAudioFormat)

Creates an audio conversion transformer to convert the format of the buffers.

### Getting the properties

let targetFormat: AVAudioFormat

The target audio format for the output buffers. It must have an AVAudioPCMFormat as its common format type.

### Applying the transformer

func applied(to: AVAudioPCMBuffer, eventHandler: EventHandler?) throws -> AVAudioPCMBuffer

Performs conversion of the input audio buffer.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Sendable
- Transformer

## See Also

### Audio components

struct AudioReader

An audio file reader.

struct AudioFeaturePrint

A stream transformer that extracts audio features from audio buffers.

