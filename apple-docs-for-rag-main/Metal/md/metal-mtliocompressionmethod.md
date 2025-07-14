

- Metal
-  MTLIOCompressionMethod 

Enumeration

# MTLIOCompressionMethod

The compression codecs that Metal supports for input/output handles.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum MTLIOCompressionMethod
```

## Overview

For more information on the individual codecs, see the Algorithm enumeration in the Compression framework.

## Topics

### Compression Codecs

case zlib

Indicates that a file uses the zlib compression algorithm codec.

case lzfse

Indicates that a file uses the LZFSE compression algorithm codec.

case lz4

Indicates that a file uses the LZ4 compression algorithm codec.

case lzma

Indicates that a file uses the LZMA compression algorithm codec.

case lzBitmap

Indicates that a file uses the LZBitmap compression algorithm codec.

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

### Asset Compression

func MTLIOCreateCompressionContext(String, MTLIOCompressionMethod, Int) -> MTLIOCompressionContext?

Creates a compression context that you use to compress data into a single file.

func MTLIOCompressionContextDefaultChunkSize() -> Int

Returns a compression chunk size you can use as a default for creating a compression context.

typealias MTLIOCompressionContext

A pointer that represents the state of a file compression session in progress.

func MTLIOCompressionContextAppendData(MTLIOCompressionContext, UnsafeRawPointer, Int)

Adds data to a compression context.

func MTLIOFlushAndDestroyCompressionContext(MTLIOCompressionContext) -> MTLIOCompressionStatus

Finishes compressing and saves the file that a compression context represents.

enum MTLIOCompressionStatus

Represents the final state of a compression context.

