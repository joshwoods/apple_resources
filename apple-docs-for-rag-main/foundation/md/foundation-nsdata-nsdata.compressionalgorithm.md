

- Foundation
- NSData
-  NSData.CompressionAlgorithm 

Enumeration

# NSData.CompressionAlgorithm

An algorithm that indicates how to compress or decompress data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum CompressionAlgorithm
```

## Overview

Choose an algorithm that best suits the needs of your app:

- NSData.CompressionAlgorithm.lzfse — The algorithm offers faster speed and generally achieves better compression than NSData.CompressionAlgorithm.zlib. However, it is slower than NSData.CompressionAlgorithm.lz4 and doesn’t compress as well as NSData.CompressionAlgorithm.lzma.

- NSData.CompressionAlgorithm.zlib — Use this algorithm if your app requires interoperability with non-Apple devices. For example, if you are transferering data to another device where it needs to be compressed or decompressed.

- NSData.CompressionAlgorithm.lz4 — Use this algorithm if speed is critical, and you’re willing to sacrifice compression ratio to achieve it.

- NSData.CompressionAlgorithm.lzma — Use this algorithm if compression ratio is critical, and you’re willing to sacrifice speed to achieve it. It is an order of magnitude slower for both compression and decompression than other choices.

## Topics

### Algorithms

case lz4

The LZ4 compression algorithm, recommended for fast compression.

case lzfse

The LZFSE compression algorithm, recommended for use on Apple platforms.

case lzma

The LZMA compression algorithm, recommended for high-compression ratio.

case zlib

The zlib compression algorithm, recommended for cross-platform compression.

case lz4

The LZ4 compression algorithm, recommended for fast compression.

case lzfse

The LZFSE compression algorithm, recommended for use on Apple platforms.

case lzma

The LZMA compression algorithm, recommended for high-compression ratio.

case zlib

The zlib compression algorithm, recommended for cross-platform compression.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Compressing and Decompressing Data

func compressed(using: NSData.CompressionAlgorithm) throws -> Self

Returns a new data object by compressing the data object’s bytes.

func decompressed(using: NSData.CompressionAlgorithm) throws -> Self

Returns a new data object by decompressing data object’s bytes.

var NSCompressionErrorMaximum: Int

The end of the range of error codes reserved for compression errors.

var NSCompressionErrorMinimum: Int

The start of the range of error codes reserved for compression errors.

var NSCompressionFailedError: Int

An error code value that indicates a failure to compress data using the provided algorithm.

var NSDecompressionFailedError: Int

An error code value that indicates a failure to decompress data using the provided algorithm.

