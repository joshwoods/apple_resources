

- Metal
-  MTLIOCompressionStatus 

Enumeration

# MTLIOCompressionStatus

Represents the final state of a compression context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLIOCompressionStatus
```

## Overview

The MTLIOFlushAndDestroyCompressionContext(_:) returns a MTLIOCompressionStatus instance to reflect the final state of a compression context.

## Topics

### Compression Result States

case complete

Indicates the compression API successfully flushed and destroyed a compression context.

case error

Indicates the compression API had an error while flushing and destroying a compression context.

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

enum MTLIOCompressionMethod

The compression codecs that Metal supports for input/output handles.

func MTLIOCompressionContextDefaultChunkSize() -> Int

Returns a compression chunk size you can use as a default for creating a compression context.

typealias MTLIOCompressionContext

A pointer that represents the state of a file compression session in progress.

func MTLIOCompressionContextAppendData(MTLIOCompressionContext, UnsafeRawPointer, Int)

Adds data to a compression context.

func MTLIOFlushAndDestroyCompressionContext(MTLIOCompressionContext) -> MTLIOCompressionStatus

Finishes compressing and saves the file that a compression context represents.

