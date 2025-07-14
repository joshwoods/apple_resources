

- Sound Analysis
- SNClassificationResult
-  timeRange 

Instance Property

# timeRange

The time span that corresponds to the result’s classifications.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var timeRange: CMTimeRange { get }
```

## Discussion

The time range’s doc://com.apple.documentation/documentation/coremedia/cmtime-u58 values are the number of audio frames at the analyzer’s sample rate. Use these time indices to determine where, in time, the result corresponds to the original audio.

A result’s time range typically refers to audio older than its most recent audio because the request gathers the data into blocks before sending them to the model.

## See Also

### Inspecting the Result

var classifications: [SNClassification]

A sorted array of the request’s top classification candidates.

class SNClassification

A type that pairs a sound classifier’s prediction with its confidence in that prediction.

func classification(forIdentifier: String) -> SNClassification?

Returns the classification for an identifier.

