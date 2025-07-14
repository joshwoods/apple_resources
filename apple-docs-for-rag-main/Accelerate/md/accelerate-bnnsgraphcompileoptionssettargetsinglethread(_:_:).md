

- Accelerate
-  BNNSGraphCompileOptionsSetTargetSingleThread(\_:\_:) 

Function

# BNNSGraphCompileOptionsSetTargetSingleThread(\_:\_:)

Sets the option for the compiled graph to execute on a single thread.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphCompileOptionsSetTargetSingleThread(
    _ options: bnns_graph_compile_options_t,
    _ value: Bool
)
```

## Parameters 

`options`  

The compilation options object.

`value`  

If `true`, the options specify single-threaded execution; otherwise, the options specify multi-threaded execution.

## Discussion

The default option is execution on multiple threads.

## See Also

### Specifying and querying compilation options

struct bnns_graph_compile_options_t

The compilation options that BNNS uses when compiling a source mlmodelc file to a graph object.

func BNNSGraphCompileOptionsMakeDefault() -> bnns_graph_compile_options_t

Returns an allocated compilation options object with default values.

func BNNSGraphCompileOptionsDestroy(bnns_graph_compile_options_t)

Destroys the specified compilation options object.

func BNNSGraphCompileOptionsSetOutputPath(bnns_graph_compile_options_t, UnsafePointer&lt;CChar>?)

Sets the option for graph compilation to generate the graph object directly to the specified file.

func BNNSGraphCompileOptionsGetOutputPath(bnns_graph_compile_options_t) -> UnsafePointer&lt;CChar>?

Returns the option for the compiled graph’s output path.

func BNNSGraphCompileOptionsSetOutputFD(bnns_graph_compile_options_t, Int32)

Sets the option for graph compilation to generate the graph object directly to the specified file descriptor.

func BNNSGraphCompileOptionsGetOutputFD(bnns_graph_compile_options_t) -> Int32

Returns the option for the compiled graph’s output file descriptor.

func BNNSGraphCompileOptionsGetTargetSingleThread(bnns_graph_compile_options_t) -> Bool

Returns the option for the compiled graph to execute on a single thread.

func BNNSGraphCompileOptionsSetOptimizationPreference(bnns_graph_compile_options_t, BNNSGraphOptimizationPreference)

Sets the option for the compiled graph to optimize for either size or performance.

func BNNSGraphCompileOptionsGetOptimizationPreference(bnns_graph_compile_options_t) -> BNNSGraphOptimizationPreference

Returns the option for the compiled graph to optimize for either size or performance.

struct BNNSGraphOptimizationPreference

Constants that describe the compilation optimization preference.

func BNNSGraphCompileOptionsSetGenerateDebugInfo(bnns_graph_compile_options_t, Bool)

Sets the option for the compiled graph to include debugging information.

func BNNSGraphCompileOptionsGetGenerateDebugInfo(bnns_graph_compile_options_t) -> Bool

Returns the option for the compiled graph to include debugging information.

var BNNSTargetSystemGeneric: BNNSTargetSystem

