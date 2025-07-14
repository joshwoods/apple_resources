

- Create ML Components
- ClassificationMetrics
-  exampleCount 

Instance Property

# exampleCount

The number of examples used to compute the metrics.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
var exampleCount: Int { get }
```

## See Also

### Getting the properties

var accuracy: Double

The number of correctly classified examples out of the total number of examples.

var labels: Set&lt;Label>

The set of labels.

var restrictToKnownLabels: Bool

A Boolean value indicating whether to restrict metrics to labels in the labels set.

