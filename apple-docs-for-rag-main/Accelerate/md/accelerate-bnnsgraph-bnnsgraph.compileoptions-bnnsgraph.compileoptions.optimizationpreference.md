

- Accelerate
- BNNSGraph
- BNNSGraph.CompileOptions
-  BNNSGraph.CompileOptions.OptimizationPreference 

Structure

# BNNSGraph.CompileOptions.OptimizationPreference

Constants that describe the compilation-optimization preference.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
struct OptimizationPreference
```

## Overview

Use the constants that this structure defines to specify whether the BNNS library compiles a graph that’s optimized either for performance or for a smaller footprint.

## Topics

### Optimization preferences

static var internalRepresentationSize: BNNSGraph.CompileOptions.OptimizationPreference

A constant that specifies compilation optimization for smallest graph size on disk.

static var performance: BNNSGraph.CompileOptions.OptimizationPreference

A constant that specifies compilation optimization for best execution performance.

## Relationships

### Conforms To

- Equatable

