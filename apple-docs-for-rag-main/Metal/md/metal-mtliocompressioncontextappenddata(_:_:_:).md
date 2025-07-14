

- Metal
-  MTLIOCompressionContextAppendData(\_:\_:\_:) 

Function

# MTLIOCompressionContextAppendData(\_:\_:\_:)

Adds data to a compression context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func MTLIOCompressionContextAppendData(
    _ context: MTLIOCompressionContext,
    _ data: UnsafeRawPointer,
    _ size: Int
)
```

## Parameters 

`context`  

An MTLIOCompressionContext instance that you create with the MTLIOCreateCompressionContext(_:_:_:) function.

`data`  

A pointer to memory that contains the data the function adds to the compression context.

`size`  

The number of bytes the function adds to the compression context from the data pointer.

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

func MTLIOFlushAndDestroyCompressionContext(MTLIOCompressionContext) -> MTLIOCompressionStatus

Finishes compressing and saves the file that a compression context represents.

enum MTLIOCompressionStatus

Represents the final state of a compression context.

