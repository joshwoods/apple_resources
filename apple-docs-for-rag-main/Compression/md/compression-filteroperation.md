

- Compression
-  FilterOperation 

Enumeration

# FilterOperation

Operations that define whether input and output filters compress or decompress data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum FilterOperation
```

## Topics

### Enumeration Cases

case compress

An operation that compresses data.

case decompress

An operation that decompresses data.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

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

enum FilterError

Errors that occur during compression.

