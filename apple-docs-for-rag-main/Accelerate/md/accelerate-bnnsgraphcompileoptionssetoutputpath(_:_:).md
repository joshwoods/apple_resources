

- Accelerate
-  BNNSGraphCompileOptionsSetOutputPath(\_:\_:) 

Function

# BNNSGraphCompileOptionsSetOutputPath(\_:\_:)

Sets the option for graph compilation to generate the graph object directly to the specified file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func BNNSGraphCompileOptionsSetOutputPath(
    _ options: bnns_graph_compile_options_t,
    _ path: UnsafePointer?
)
```

## Parameters 

`options`  

The compilation options object.

`path`  

The destination file path. Pass `nil` to reset to the default behavior of strictly in-memory graph generation.

## Discussion

Use this option to specify that the graph BNNSGraphCompileFromFile(_:_:_:) returns is a read-only memory-mapped file.

The option reduces the memory that compilation requires because BNNS doesn’t require the full set of graph weights to be memory resident.

The generated file has 0600 permissions (read and write by the user only).

Note that the BNNSGraphCompileOptionsSetOutputFD(_:_:) function overrides this option.

## See Also

### Specifying and querying compilation options

struct bnns_graph_compile_options_t

The compilation options that BNNS uses when compiling a source mlmodelc file to a graph object.

func BNNSGraphCompileOptionsMakeDefault() -> bnns_graph_compile_options_t

Returns an allocated compilation options object with default values.

func BNNSGraphCompileOptionsDestroy(bnns_graph_compile_options_t)

Destroys the specified compilation options object.

func BNNSGraphCompileOptionsGetOutputPath(bnns_graph_compile_options_t) -> UnsafePointer&lt;CChar>?

Returns the option for the compiled graph’s output path.

func BNNSGraphCompileOptionsSetOutputFD(bnns_graph_compile_options_t, Int32)

Sets the option for graph compilation to generate the graph object directly to the specified file descriptor.

func BNNSGraphCompileOptionsGetOutputFD(bnns_graph_compile_options_t) -> Int32

Returns the option for the compiled graph’s output file descriptor.

func BNNSGraphCompileOptionsSetTargetSingleThread(bnns_graph_compile_options_t, Bool)

Sets the option for the compiled graph to execute on a single thread.

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

