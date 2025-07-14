

- Metal
-  MTLIOFlushAndDestroyCompressionContext(\_:) 

Function

# MTLIOFlushAndDestroyCompressionContext(\_:)

Finishes compressing and saves the file that a compression context represents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func MTLIOFlushAndDestroyCompressionContext(_ context: MTLIOCompressionContext) -> MTLIOCompressionStatus
```

## Parameters 

`context`  

A compression context that you create with the MTLIOCreateCompressionContext(_:_:_:) function.

## Return Value

An MTLIOCompressionStatus instance.

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

enum MTLIOCompressionStatus

Represents the final state of a compression context.

