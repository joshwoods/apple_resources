

- Sound Analysis
-  SNClassificationResult 

Class

# SNClassificationResult

A result that contains the highest-ranking classifications in a time range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class SNClassificationResult
```

## Overview

An `SNClassificationResult` represents the predictions that a sound classification model made for a time span in an audio file or stream. Each result contains one or more classification predictions and a time range within the audio data.

An audio analyzer, such as SNAudioFileAnalyzer and SNAudioStreamAnalyzer, produces an `SNClassificationResult` each time it recognizes a sound for any of its SNClassifySoundRequest instances.

## Topics

### Inspecting the Result

var timeRange: CMTimeRange

The time span that corresponds to the result’s classifications.

var classifications: [SNClassification]

A sorted array of the request’s top classification candidates.

class SNClassification

A type that pairs a sound classifier’s prediction with its confidence in that prediction.

func classification(forIdentifier: String) -> SNClassification?

Returns the classification for an identifier.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- SNResult

## See Also

### Sound classification requests

Classifying Live Audio Input with a Built-in Sound Classifier

Detect and identify hundreds of sounds by using a trained classifier.

class SNClassifySoundRequest

A request that classifies sound using a Core ML model.

