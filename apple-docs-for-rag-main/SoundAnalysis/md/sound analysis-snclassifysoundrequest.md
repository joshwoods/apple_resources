

- Sound Analysis
-  SNClassifySoundRequest 

Class

# SNClassifySoundRequest

A request that classifies sound using a Core ML model.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class SNClassifySoundRequest
```

## Mentioned in 

Classifying Sounds in an Audio File

Classifying Sounds in an Audio Stream

## Overview

An `SNClassifySoundRequest` represents a specific sound classification model. Analyze audio data with a sound classification model by:

1.  Creating an `SNClassifySoundRequest`, either with the Sound Analysis model, or by providing your custom Core ML model.

2.  Adding the sound request to an SNAudioFileAnalyzer or SNAudioStreamAnalyzer to process an audio file or stream, respectively.

```
func makeRequest(_ customModel: MLModel? = nil) throws -> SNClassifySoundRequest {
    // If applicable, create a request with a custom sound classification model.
    if let model = customModel {
        let customRequest = try SNClassifySoundRequest(mlModel: model)
        return customRequest
    }

    // Create a request with the Sound Analysis model.
    let version1 = SNClassifierIdentifier.version1
    let request = try SNClassifySoundRequest(classifierIdentifier: version1)

    return request
}

let classifySoundRequest = try makeRequest()

// Prints every label in the request's sound classification model.
print(classifySoundRequest.knownClassifications)
```

For more information about creating and using classify sound requests, see:

- Classifying Sounds in an Audio File

- Classifying Sounds in an Audio Stream

## Topics

### Creating a Request

init(mlModel: MLModel) throws

Creates a request that uses a custom sound classification model.

init(classifierIdentifier: SNClassifierIdentifier) throws

Creates a request that uses the framework’s built-in sound classification model.

struct SNClassifierIdentifier

An identifier that represents the versions of the framework’s sound classifier.

### Configuring a Request

var overlapFactor: Double

The amount of overlap between successive analysis windows when the model operates on a fixed-size audio block.

var windowDuration: CMTime

The duration of the audio buffer the request sends to the underlying sound classifier for each prediction.

### Inspecting a Request

var knownClassifications: [String]

A string array that contains every prediction label in the request’s underlying sound classifier model.

enum SNTimeDurationConstraint

Defines the time duration windows the request’s underlying sound classifier accepts with a range, or an array, of durations.

### Instance Properties

var windowDurationConstraint: SNTimeDurationConstraint

A range or list of sound duration times the request’s underlying sound classifier supports.

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
- SNRequest

## See Also

### Sound classification requests

Classifying Live Audio Input with a Built-in Sound Classifier

Detect and identify hundreds of sounds by using a trained classifier.

class SNClassificationResult

A result that contains the highest-ranking classifications in a time range.

