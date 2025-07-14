

- Sound Analysis
- SNClassificationResult
-  classification(forIdentifier:) 

Instance Method

# classification(forIdentifier:)

Returns the classification for an identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func classification(forIdentifier identifier: String) -> SNClassification?
```

## Parameters 

`identifier`  

A sound classification label.

## Return Value

A sound classification with a corresponding identifier if it exists in the result; otherwise, `nil`.

## Discussion

The `identifier` parameter corresponds to the identifier property in an SNClassification.

## See Also

### Inspecting the Result

var timeRange: CMTimeRange

The time span that corresponds to the result’s classifications.

var classifications: [SNClassification]

A sorted array of the request’s top classification candidates.

class SNClassification

A type that pairs a sound classifier’s prediction with its confidence in that prediction.

