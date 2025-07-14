

- Foundation
-  NSCompressionFailedError 

Global Variable

# NSCompressionFailedError

An error code value that indicates a failure to compress data using the provided algorithm.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var NSCompressionFailedError: Int { get }
```

## See Also

### Compressing and Decompressing Data

func compressed(using: NSData.CompressionAlgorithm) throws -> Self

Returns a new data object by compressing the data object’s bytes.

func decompressed(using: NSData.CompressionAlgorithm) throws -> Self

Returns a new data object by decompressing data object’s bytes.

enum CompressionAlgorithm

An algorithm that indicates how to compress or decompress data.

var NSCompressionErrorMaximum: Int

The end of the range of error codes reserved for compression errors.

var NSCompressionErrorMinimum: Int

The start of the range of error codes reserved for compression errors.

var NSDecompressionFailedError: Int

An error code value that indicates a failure to decompress data using the provided algorithm.

