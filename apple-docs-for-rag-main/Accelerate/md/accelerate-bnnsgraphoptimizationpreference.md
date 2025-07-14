

- Accelerate
-  BNNSGraphOptimizationPreference 

Structure

# BNNSGraphOptimizationPreference

Constants that describe the compilation optimization preference.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSGraphOptimizationPreference
```

## Topics

### Optimization preferences

init(UInt32)

Creates a new instance.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

### Instance properties

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSGraphOptimizationPreferenceIRSize: BNNSGraphOptimizationPreference

A constant that specifies compilation optimization for smallest graph size on disk.

var BNNSGraphOptimizationPreferencePerformance: BNNSGraphOptimizationPreference

A constant that specifies compilation optimization for best execution performance.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func BNNSGraphCompileOptionsSetTargetSingleThread(bnns_graph_compile_options_t, Bool)

Sets the option for the compiled graph to execute on a single thread.

func BNNSGraphCompileOptionsGetTargetSingleThread(bnns_graph_compile_options_t) -> Bool

Returns the option for the compiled graph to execute on a single thread.

func BNNSGraphCompileOptionsSetOptimizationPreference(bnns_graph_compile_options_t, BNNSGraphOptimizationPreference)

Sets the option for the compiled graph to optimize for either size or performance.

func BNNSGraphCompileOptionsGetOptimizationPreference(bnns_graph_compile_options_t) -> BNNSGraphOptimizationPreference

Returns the option for the compiled graph to optimize for either size or performance.

func BNNSGraphCompileOptionsSetGenerateDebugInfo(bnns_graph_compile_options_t, Bool)

Sets the option for the compiled graph to include debugging information.

func BNNSGraphCompileOptionsGetGenerateDebugInfo(bnns_graph_compile_options_t) -> Bool

Returns the option for the compiled graph to include debugging information.

var BNNSTargetSystemGeneric: BNNSTargetSystem

