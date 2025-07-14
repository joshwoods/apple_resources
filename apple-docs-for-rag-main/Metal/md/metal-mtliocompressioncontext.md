

- Metal
-  MTLIOCompressionContext 

Type Alias

# MTLIOCompressionContext

A pointer that represents the state of a file compression session in progress.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLIOCompressionContext = UnsafeMutableRawPointer
```

## See Also

### Asset Compression

func MTLIOCreateCompressionContext(String, MTLIOCompressionMethod, Int) -> MTLIOCompressionContext?

Creates a compression context that you use to compress data into a single file.

enum MTLIOCompressionMethod

The compression codecs that Metal supports for input/output handles.

func MTLIOCompressionContextDefaultChunkSize() -> Int

Returns a compression chunk size you can use as a default for creating a compression context.

func MTLIOCompressionContextAppendData(MTLIOCompressionContext, UnsafeRawPointer, Int)

Adds data to a compression context.

func MTLIOFlushAndDestroyCompressionContext(MTLIOCompressionContext) -> MTLIOCompressionStatus

Finishes compressing and saves the file that a compression context represents.

enum MTLIOCompressionStatus

Represents the final state of a compression context.

