

- Core ML
- MLUpdateContext
-  metrics 

Instance Property

# metrics

The training metrics of the model for the update task, contained in a dictionary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
var metrics: [MLMetricKey : Any] { get }
```

## Discussion

Use the MLMetricKey to access the values within the dictionary.

## See Also

### Evaluating the Update

class MLMetricKey

A key for the metrics dictionary in an update context.

