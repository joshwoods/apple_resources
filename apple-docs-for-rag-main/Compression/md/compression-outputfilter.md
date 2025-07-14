

- Compression
-  OutputFilter 

Class

# OutputFilter

An encoder-decoder that writes output data to a stream.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
class OutputFilter
```

## Topics

### Initializers

Creates an output filter for compressing or decompressing data.

init(FilterOperation, using: Algorithm, bufferCapacity: Int, writingTo: (Data?) throws -> Void) throws

Creates an output filter that can be used to compress or decompress data.

### Instance Methods

func write&lt;D>(D?) throws

Writes data to the output filter.

func finalize() throws

Finalizes the stream by flushing all the remaining data in the stream.

## See Also

### Objects that simplify multiple-step compression

Compressing and decompressing data with input and output filters

Compress and decompress streamed or from-memory data, using input and output filters.

Compressing and decompressing files with stream compression

Perform compression for all files and decompression for files with supported extension types.

class InputFilter

An encoder-decoder that reads input data from a stream.

enum Algorithm

Algorithms used for compression or decompression.

enum FilterError

Errors that occur during compression.

enum FilterOperation

Operations that define whether input and output filters compress or decompress data.

