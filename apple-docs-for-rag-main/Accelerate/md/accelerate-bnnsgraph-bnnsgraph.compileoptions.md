

- Accelerate
- BNNSGraph
-  BNNSGraph.CompileOptions 

Structure

# BNNSGraph.CompileOptions

The compilation options that BNNS uses when compiling a source mlmodelc file to a graph object.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
struct CompileOptions
```

## Overview

Call init(compileFromPath:functionName:options:) to create a default options structure and then set properties such as optimizationPreference to specify individual options.

## Topics

### Creating a compilation options structure

init()

Creates an allocated compilation-options object with default values.

init(useSingleThread: Bool, generateDebugInfo: Bool, optimizationPreference: BNNSGraph.CompileOptions.OptimizationPreference)

Creates an allocated compilation-options object with the specified values.

### Specifying and querying compilation options

var useSingleThread: Bool

A Boolean value that specifies whether the graph executes on one thread.

var generateDebugInfo: Bool

A Boolean value that specifies whether the generated graph includes debug info.

var optimizationPreference: BNNSGraph.CompileOptions.OptimizationPreference

A constant that specifies the graph compilation-optimization preferences.

### Specifying the optimization preference

struct OptimizationPreference

Constants that describe the compilation-optimization preference.

## See Also

### Creating a graph context

init(compileFromPath: String, functionName: String?, options: BNNSGraph.CompileOptions) async throws

Returns a new context that wraps a graph object representing the compiled mlmodelc file.

