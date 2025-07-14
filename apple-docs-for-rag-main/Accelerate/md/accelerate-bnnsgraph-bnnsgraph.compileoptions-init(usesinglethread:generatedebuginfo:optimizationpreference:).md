

- Accelerate
- BNNSGraph
- BNNSGraph.CompileOptions
-  init(useSingleThread:generateDebugInfo:optimizationPreference:) 

Initializer

# init(useSingleThread:generateDebugInfo:optimizationPreference:)

Creates an allocated compilation-options object with the specified values.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
init(
    useSingleThread: Bool = false,
    generateDebugInfo: Bool = false,
    optimizationPreference: BNNSGraph.CompileOptions.OptimizationPreference = .performance
)
```

## Parameters 

`useSingleThread`  

A Boolean value that specifies whether the graph executes on one thread.

`generateDebugInfo`  

A Boolean value that specifies whether the generated graph includes debug info.

`optimizationPreference`  

A constant that specifies the graph compilation-optimization preferences.

## See Also

### Creating a compilation options structure

init()

Creates an allocated compilation-options object with default values.

