

- Compression
-  FilterError 

Enumeration

# FilterError

Errors that occur during compression.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum FilterError
```

## Topics

### Enumeration Cases

case invalidData

An error that indicates invalid data passed to the encoder-decoder.

case invalidState

An error that indicates a filter failed to initialize, or that it has an invalid internal stare or parameters.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Objects that simplify multiple-step compression

Compressing and decompressing data with input and output filters

Compress and decompress streamed or from-memory data, using input and output filters.

Compressing and decompressing files with stream compression

Perform compression for all files and decompression for files with supported extension types.

class InputFilter

An encoder-decoder that reads input data from a stream.

class OutputFilter

An encoder-decoder that writes output data to a stream.

enum Algorithm

Algorithms used for compression or decompression.

enum FilterOperation

Operations that define whether input and output filters compress or decompress data.

