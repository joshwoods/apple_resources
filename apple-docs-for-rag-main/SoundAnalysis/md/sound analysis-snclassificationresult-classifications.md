

- Sound Analysis
- SNClassificationResult
-  classifications 

Instance Property

# classifications

A sorted array of the request’s top classification candidates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var classifications: [SNClassification] { get }
```

## Discussion

`SNClassificationResult` sorts its classifications in descending confidence score order.

## See Also

### Inspecting the Result

var timeRange: CMTimeRange

The time span that corresponds to the result’s classifications.

class SNClassification

A type that pairs a sound classifier’s prediction with its confidence in that prediction.

func classification(forIdentifier: String) -> SNClassification?

Returns the classification for an identifier.

