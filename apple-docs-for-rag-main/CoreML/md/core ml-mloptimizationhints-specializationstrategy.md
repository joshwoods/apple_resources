

- Core ML
- MLOptimizationHints
-  specializationStrategy 

Instance Property

# specializationStrategy

Optimization strategy for the model specialization.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var specializationStrategy: MLOptimizationHints.SpecializationStrategy
```

## Discussion

Core ML segments the model’s compute graph and specializes each segment for the target compute device. This process can affect the model loading time and the prediction latency.

Use this option to tailor the specialization strategy for your model.

