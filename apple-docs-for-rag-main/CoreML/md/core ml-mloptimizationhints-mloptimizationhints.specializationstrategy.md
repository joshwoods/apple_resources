

- Core ML
- MLOptimizationHints
-  MLOptimizationHints.SpecializationStrategy 

Enumeration

# MLOptimizationHints.SpecializationStrategy

The optimization strategy for the model specialization.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum SpecializationStrategy
```

## Topics

### Enumeration Cases

case `default`

The strategy that should work well for most applications.

case fastPrediction

Prefer the prediction latency at the potential cost of specialization time, memory footprint, and the disk space usage of specialized artifacts.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

