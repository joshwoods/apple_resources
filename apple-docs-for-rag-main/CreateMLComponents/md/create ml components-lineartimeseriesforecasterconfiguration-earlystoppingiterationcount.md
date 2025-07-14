

- Create ML Components
- LinearTimeSeriesForecasterConfiguration
-  earlyStoppingIterationCount 

Instance Property

# earlyStoppingIterationCount

The number of iterations to use when evaluating whether to stop early.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var earlyStoppingIterationCount: Int
```

## Discussion

The `fitted` method will stop if no significant progress is made for this many iterations. Significant progress happens when the validation error decreases by at least `convergenceThreshold`.

Note

Early stopping only happens when using the `fitted` method with validation data.

