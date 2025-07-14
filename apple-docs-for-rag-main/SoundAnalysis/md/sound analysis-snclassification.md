

- Sound Analysis
-  SNClassification 

Class

# SNClassification

A type that pairs a sound classifier’s prediction with its confidence in that prediction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class SNClassification
```

## Overview

An `SNClassification` represents a single sound classification prediction, and the sound classifier model’s confidence in that prediction.

## Topics

### Inspecting a Classification

var identifier: String

A prediction label that’s one of the classifications a sound classifier’s underlying model defines.

var confidence: Double

The confidence value the model has in its prediction.

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

## See Also

### Inspecting the Result

var timeRange: CMTimeRange

The time span that corresponds to the result’s classifications.

var classifications: [SNClassification]

A sorted array of the request’s top classification candidates.

func classification(forIdentifier: String) -> SNClassification?

Returns the classification for an identifier.

