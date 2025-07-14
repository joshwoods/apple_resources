

- Compression
-  Algorithm 

Enumeration

# Algorithm

Algorithms used for compression or decompression.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum Algorithm
```

## Topics

### Enumeration Cases

case brotli

The Brotli compression algorithm, which is recommended for text compression.

case lz4

The LZ4 compression algorithm, which is recommended for fast compression.

case lzbitmap

The LZBITMAP compression algorithm, which is designed to exploit the vector instruction set of current CPUs.

case lzfse

The LZFSE compression algorithm, which is recommended for use on Apple platforms.

case lzma

The LZMA compression algorithm, which is recommended for high-compression ratio.

case zlib

The zlib compression algorithm, which is recommended for cross-platform compression.

## Relationships

### Conforms To

- CaseIterable
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

enum FilterError

Errors that occur during compression.

enum FilterOperation

Operations that define whether input and output filters compress or decompress data.

