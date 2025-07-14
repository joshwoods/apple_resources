

- Metal
-  MTLIOCreateCompressionContext(\_:\_:\_:) 

Function

# MTLIOCreateCompressionContext(\_:\_:\_:)

Creates a compression context that you use to compress data into a single file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS

``` source
func MTLIOCreateCompressionContext(
    _ path: String,
    _ type: MTLIOCompressionMethod,
    _ chunkSize: Int
) -> MTLIOCompressionContext?
```

## Parameters 

`path`  

A location in the file system where the function creates the new, compressed file.

`type`  

A compression codec the function uses to compress data resource file’s compression format.

`chunkSize`  

The number of uncompressed bytes the compression codec compresses at a time.

## See Also

### Asset Compression

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

enum MTLIOCompressionStatus

Represents the final state of a compression context.

